# Marking Guide for AI'24 - Project 4 - Minecraft (Prolog)

This document explains the automarking framework and system used for Project 3 - Minecraft in Prolog.

In order to understand the output from the automarker, there are two distinct components:

1. the different test set cases we graded with; and
2. the dimensions each tests is evaluated/checked against.

The automarker will produce a YAML file describing the outcome of each single test in each test set. See below for an example of a part of such YAML file.

- [Marking Guide for AI'24 - Project 4 - Minecraft (Prolog)](#marking-guide-for-ai24---project-4---minecraft-prolog)
  - [Consult error-free](#consult-error-free)
  - [Test cases](#test-cases)
  - [Grading dimensions](#grading-dimensions)
    - [Completeness](#completeness)
    - [Redundancy](#redundancy)
    - [Soundness](#soundness)
  - [Overall score/marks](#overall-scoremarks)
  - [Report](#report)
    - [Forbidden predicates](#forbidden-predicates)
    - [Predicate dependencies and best modes](#predicate-dependencies-and-best-modes)

## Consult error-free

Of course the very first and most basic requirement to get any marks is that your codebase compiles error free, so that the automarker can load it up as a library in full:

```
* Your code **must consult and run _error-free_ on [SWI-Prolog](https://www.swi-prolog.org/)**. Staff will not debug/fix any code.
```

This is super easy to check, you just consult your solution file and it should report NO error whatsoever:

```shell
$ swipl
Welcome to SWI-Prolog (threaded, 64 bits, version 8.4.2)
SWI-Prolog comes with ABSOLUTELY NO WARRANTY. This is free software.
Please run ?- license. for legal details.

For online help and background, visit https://www.swi-prolog.org
For built-in help, use ?- help(Topic). or ?- apropos(Word).

?- ['minecraft.pl'].
true.
```

An alternative way is to consult your file when starting SWI-Prolog:

```shell
$ swipl minecraft.pl
Welcome to SWI-Prolog (threaded, 64 bits, version 8.4.2)
SWI-Prolog comes with ABSOLUTELY NO WARRANTY. This is free software.
Please run ?- license. for legal details.

For online help and background, visit https://www.swi-prolog.org
For built-in help, use ?- help(Topic). or ?- apropos(Word).

?-
```

The above cases report no error, so file `minecraft.pl` have been consulted (i.e., loaded) successfully.

In contrast, here is an example of a file that is _not_ error free:

```shell
$ swipl
Welcome to SWI-Prolog (threaded, 64 bits, version 8.4.2)
SWI-Prolog comes with ABSOLUTELY NO WARRANTY. This is free software.
Please run ?- license. for legal details.

For online help and background, visit https://www.swi-prolog.org
For built-in help, use ?- help(Topic). or ?- apropos(Word).

?- ['minecraft.pl'].
ERROR: /mnt/ssardina-volume/cosc1125-1127-AI/AI23/p3-prolog/submissions/bad/minecraft.pl:146:35: Syntax error: Unexpected end of file
true.
```

or simply:

```shell
$ swipl minecraft.pl
ERROR: /mnt/ssardina-volume/cosc1125-1127-AI/AI23/p3-prolog/submissions/bad/minecraft.pl:146:35: Syntax error: Unexpected end of file
Welcome to SWI-Prolog (threaded, 64 bits, version 8.4.2)
SWI-Prolog comes with ABSOLUTELY NO WARRANTY. This is free software.
Please run ?- license. for legal details.

For online help and background, visit https://www.swi-prolog.org
For built-in help, use ?- help(Topic). or ?- apropos(Word).

?-
```

One can see in the above cases that the file has syntax problems in line 164 and hence it yields ERROR. A file like this will not be marked and will attract zero marks, as per spec. When this happens the report will signal it with the following feedback:

```
- 'Solution file consulted with error (this should never happen): syntax_error(end_of_file)'
```

(Note that interactive SWI-Prolog and unit testing framework will still load the file _partially_ and reporting the error, so as to help in the debugging. But ultimately the codebase has to be error-free.)

## Test cases

Each exercise is tested against three _sets_ of test cases, each compromising of various _single tests_.

So, for each exercise `N`, there are three test sets:

* `exN_spec`: these contain the exact tests which we provided in the test file in the project repository.
* `exN_core`: these contain a similar set of tests which use a _different_ percept generated from the Agent in the City game server. They check for generality of solution, but should be not be harder or easier than `exN_spec`.
* `exN_handcrafted`: these contain a set of handcrafted tests which use a manually defined percept. These are designed to check edge/special cases and unusual scenarios.

Each test set is associated a number of _marks_, all test sets in the project sum up to 100. For example, for Exercise 1 (`N=1`) each of the above three test set is worth 5 marks, for a total of 15 marks (which is the weight of Exercise 1). Each single test within a test set is assigned a number of _points_: to get all the marks of the test set, one has to collect all points in it. So, if a test set is worth 5 marks and has 10 single tests of 1 point each, collecting 5 points amounts to 2.5 marks for the test set.

## Grading dimensions

For Prolog, each standard single test case takes the form of a query. The expected answer is the expected results of the query. The query results can be either a boolean value (if no variables are involved in the query), or one or more sets of bindings for the free variables in the query (which we will refer to as a solution). For all queries, we check three properties: _completeness_, _redundancy_, and _soundness_.

### Completeness

This is where we check whether the implementation is complete, that is, it yields all the right solutions. For a boolean result, this is a binary `true`/`false` check.

For a solution (answers with bindings), the calculation is more complex. In general, a query may have a _set_ of intended solutions (each with different bindings), so the automarker checks how many of them are returned as answers, and award partial marks proportional to the number of solutions found.

In some cases, though, we are more interested in some variable bindings than others. In this case, we sometimes award partial marks to solutions which are not fully correct (they are not exactly one of the expected answers), but are close to one correct answer. For example, if you have the expected answer: `A = apple, B  = banana, X = 3`, and the student answer: `A = apple, B = banana, X = 4`, this may be eligible for _partial_ marks (even though, technically, the answer is incorrect).

An implementation which is (fully) _complete_ is given 90% of the total marks for the question. These marks are indicated in the marking report by lines such as:\

```
Test N: [P] - Completness: X/Y
```

where `N` is the ID of the test case, `P` is the number of points awarded to this answer, `X` is the number of solutions generated (that were able to be at least partially matched to the expected set), and `Y` is the number of solutions expected  (always 1 for a boolean output).

### Redundancy

We next check for answers redundancy. This is important, as inefficient Prolog programs can often generate large numbers of identical solutions, which is not particularly useful.

We simply identify if there are any duplicates in the solution set generated. If not, the answer gets the remaining 10% of the total marks for the question. These marks are indicated in the marking report by lines such as:

```
Test N: [P] - No redundant answers found! :-)
```

or

```
Test N: [P] - Redundant answers found...
```

Where `N` is the ID of the test case, and `P` is the number of points awarded to this answer for redundancy.

To be eligible for these marks, the query must have non-zero completeness; i.e. At least one correct solution must have been generated. This is to avoid trivial programs from receiving these marks just because they always return one answer (e.g. `true`).

### Soundness

Finally, we check if the answer is _sound_, that is, whether it never yields _incorrect_ answers. Unsoundness is indeed a serious problem: producing wrong solutions is generally worse than failing to produce some expected solutions. As a result, if there are any unexpected solutions found (i.e., those that cannot even be partially matched against an expected solution), the score is reduced by 70% of the marks that you have obtained in the completeness and redundancy stages.

Soundness checks are not applied to boolean solutions (as it is the same as the completeness check).

These marks are indicated in the marking report by lines such as:

```
Test N: [-P] - Incorrect answers found... (e.g., S)
```

where `N` is the ID of the test case, `P` is the number of points subtracted from this answer for soundness failure, and `S` is one example of a solution that was unexpected.

## Overall score/marks

Ultimately, the points received by the student for a standard test case is given by the following formula:

$$points = (0.9\cdot t\cdot p_c + 0.1\cdot m \cdot b_r) \cdot 0.3\cdot b_s$$

where:

* $t$ is the total points allocated to that test case,
* $p_c$ is the ratio of correct solutions generated (including partial matches) -- 1 is all expected solutions generated,
* $b_r$ is a binary redundancy flag set to $1$ if _no redundant_ solutions were found, and
* $b_s$ is a binary soundness flag set to $1$ if any _unsound_ solutions were found (which means -70% discount if wrong answers are returned).

This is indicated in the marking report by lines such as:

```
Test N: [P/T] - Final points collected
```
where `N` is the ID of the test case, `P` is the number of points received by the submission, and `T` is the total points available.


## Report

The automarker will produce a YAML file with the summary of the results for each test set. The report will follow the framework above.

An example of the section of test set `ex2_core` (core test set for Exercise 2) is as follows:

```
 ex1_handcrafted:
    desc: checks tools_for_items/2 predicate
    points: 3.0
    points_available: 3
    bonus_available: 0.5
    marks: 8.0
    marks_available: 8
    feedback:
    - 'Test 1: (++,--) with; failure'
    - 'Test 1: [1.00] - Correct answer! :-)'
    - 'Test 1: [1.00/1.00] - Final points collected'
    - 'Test 2: (++,--) check; single answer'
    - 'Test 2: [0.90] - Completeness: 1/1'
    - 'Test 2: [0.10] - No redundant answers found! :-)'
    - 'Test 2: [1.00/1.00] - Final points collected'
    - 'Test 3: (++,--) check; multiple tools for one item'
    - 'Test 3: [0.00] - Completeness: 0/1'
    - 'Test 3: [0.00] - No correct answers given, not eligible for redundancy marks'
    - 'Test 3: [-0.00] - Incorrect answers found... (e.g., {''T'': [''t1'', ''t2'']})
      :-( )'
    - 'Test 3: [0.00/0.50] - Final points collected (BONUS)'
    - 'Test 4: (++,--) check; tool that cannot be made'
    - 'Test 4: [0.90] - Completeness: 1/1'
    - 'Test 4: [0.10] - No redundant answers found! :-)'
    - 'Test 4: [1.00/1.00] - Final points collected'
```

In this fragment, there are 4 single tests. Each has been checked for completeness, redundancy, and soundness. The first line of each single test is a a simple explanation of what the test is about. In the above fragment, the student has collected all 3 points available, yielding 8 marks (out of 8), but has not attracted the 0.5 bonus points in Test 3.

### Forbidden predicates

When a test is found to use a forbidden predicate, as per the "Language restrictions and guidelines ⚡" section in the project spec, the test will attract no points and be reported as follows:

```
    - 'Test 2: [0.00] - Test failed due to exception: A forbidden predicate has been
      used: {''findall''}'
```

In this case, the test used the `findall/3` predicate which was not allowed.

It is the MINIMUM expectation to adhere to these rules. No partial marks will be awarded when these rules are broken or ignored.


### Predicate dependencies and best modes

In general, we would test the code of each question using correct implementation of dependencies. This is more notorious and relevant in Exercise 4, in which you would heavily rely on previous exercises.

So, when we tested your Exercise 4 `required_raw_ingredients/2` implementation, we would use correct solutions for all previous predicates.

It turned out, however, that same student submissions for Exercise 4 performed better with their own, non-correct, implementation of previous questions.

So, we would run each test set in two modes: 

1. using our perfect implementation of previous predicates;
2. using your previous predicates, even if buggy and not fully correct.

We would then take the one that achieves more points. You will see that in the report as follows:

```
   best_mode: You scored the most points when we ran your code with your implementations for prior questions, so all results for this question are using your implementations.
```


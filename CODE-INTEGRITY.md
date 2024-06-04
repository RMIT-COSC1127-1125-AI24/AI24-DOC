## In a code assignment/project, how do I make sure I do not go against academic integrity?

**Good question!**

The simple answer is: your solution has to be **your own work**. In terms of code, your code **must be written entirely by yourself**.

* As a rule, you should never look at or run anyone else's code for the assignment, whether the code was written by someone currently in the class, or someone who took it previously, even at another university. 

A very smart strategy to protect yourself against breaching the Course Honesty Policy is this one: _**never search a solution (or part of it) for the project problem you are meant to solve**_.

* Never search "_A* pacman_" or even "_A* in Python_" or similar, because that is what you need to produce _entirely_ by yourself. 
* If you do, you are only tricking yourself, jeopardizing your opportunity to learn, breaching the Course Honesty Policy, and putting you at risk of going through the University academic misconduct process. 
* In most cases, once you saw someone else's solution, it is **often too late** for you to come up with YOUR entire solution (which is when you actually learn). It is easy to understand something somebody already solved, the difficult but rewarding task is to build the solution yourself (remember NP problems??) !

**Adapting someone else's solution does not make it your own work**. So, if you take, say, an A* implementation (even if not for Pacman) and **adapting** it to your (Pacman) needs, then **the solution is _not_ your own work anymore** and may not be submitted without breaching Academic Integrity. That code is not auxiliary code anymore, it is the code you are meant to produce in your learning journey. 


Said so, there are **many things you can do safely** and you are encouraged to! Let’s discuss them...

1. **Reading pseudo-code** for a technique, from text-books, papers, the web, or slides, is completely OK and even expected (e.g., reading and studying the pseudo-code for minimax or A* algorithms). If you use a source (e.g., text-book) very closely, for example, converting the pseudocode of A* in the textbook to Python, academic integrity demands that you cite the source (in a comment). You will not be penalized for including such a comment ("_Based on pseudo-code in book X, page Y_”); on the contrary, the citation may help us to understand why your implementation is so similar to someone else's, in case they use and cite the same source.
2. **Using existing libraries and tools to support auxiliary tasks** that do not involve solving the problem (or an important part of it) we are interested in. 

    * For example, **you can use Python libraries for generic tasks** (e.g., math libraries, arrays, etc.); such tasks are not what the project is about and we are not learning how to build those libraries. You can use those libraries off-the-shelf. 
    * However, if you find **a library that solves your problem or a non-auxiliarly part of it**, then you **may not use it**. For example, if you find a library of search algorithms, then it is obviously not acceptable to use it, as then you are not solving the problem, you are _reusing someone else's solution_: they won, they know, you don't. :-)

3. You can also **reuse generic code for specific auxiliary tasks** that you may need, in the path of building your solution to the project problem. For example, if you need to extract the odd numbers you can use:

    ```python
        oddNums = [x for x in nums if x % 2 == 1] 
    ```

    or variations of it that are everywhere on the web, as long as you understand what that code is doing. The fact is that that code is auxiliary support code, it does not constitute the core solution to the actual problem you are to solve. So generic Python code is fine to reuse, but remember you need to understand it and unless very trivial _acknowledge it in your code (with a comment)_.

4. You are **encouraged to discuss with your peers**, even your solutions, but **always at the verbal level**, never sharing or showing code (even snippets), and never seeing step-by-step the code of your friend. 

    * It is totally fine to exchange ideas, insights, or tips like: "_why don't you try a dictionary to store X instead of an array?_" or "_remember to check for goal after you extract a node from the open list, not when you expand_" or "_be careful with X, I had a problem when ...._", or "_use library X to do Y, it works much better than Z_", etc.
    * If you just keep the collaboration at the speech level, it is very difficult to do anything wrong; if on the other hand you show or pass code, then you are putting you and your friend into a big risk and missing out in the learning. Don't do it, not worth it. 
    * Of course, if it is just about Python, it is OK to go over code, for example it is OK to explain to your friend how you do list comprehension, that is, again, auxiliary code.

 
Observe you it is totally fine to **research general techniques or techniques for different problems** that you may find useful **importing into Pacman problems**. For example, you may research what is used in pathfinding or in TSP or in network flow problems. Then you may adapt and import those techniques to your specific task. If the problem you researched had nothing to do with Pacman, then you are safe. You will of course, as courtesy and ethical behavior, then explain and acknowledge in your report what you took from where and explain how that was helpful for your solution. For example, in the past, a student reported this which was just perfect:

```
Tried to use the heuristics from question 6. Heuristic was not
acceptable..
......
Realized that ..........
........
Since I now have a fixed the XXXXXXX distance problem, I did some 
research online on possible heuristics which may help.
First off, I started with looking up heuristics for problem XYZ since it is
similar.
____________________________________________________________
Solution 1 (commented out in searchAgents.py line 524 - 536) 
------------------------------------------------------------

https://abc.cde.fgh.sk/abc-cit/butka/abc.pdf
I adapted the logic behind section 3.1 (ABC XYZ) to see if it
will work. Was able to reduce the nodes expanded to 12372 nodes (2/4)

Solution 2 and 3 were inspired by the behaviour I observed in the the
Corner's problem (Question 6)....
.......
```

As one can see, the student was faced with a problem, as the naive solution did not work well. Then worked out a fix for part of it and then researched techniques in a completely different problem XYZ that the student thought could be imported into Pacman. He adapted it and later did a few changes to make it specific for the Pacman problem at hand. **JUST PERFECT!** :-)

Finally, borrowing  related [entry from Stackoverflow](http://meta.stackoverflow.com/questions/334822/how-do-i-ask-and-answer-homework-questions) on how to ask questions about assignment, here are some good strategies:

* **Make a good faith attempt to solve the problem yourself first**. If you can't see enough work on your part, then there is probably a problem.
* **Ask about specific problems with your existing implementation**. If you can't do that yet because you have nothing, then there is probably a problem.
* **Admit that the question is homework**. Always be upfront when you ask about assignments (you can structure your question this way: “_How can I do …? I'm trying to do this as part of … which is a homework problem. This is my attempt so far: ..._”).
* **Never use code you don't understand**. It definitely won't help you later (after school, in later assignments, on tests, etc.) and it could be, at best, very embarrassing if you are asked to explain code you turned in.

Observe that an assignment in a course is **not an open source project** and it is not acceptable to search for help in web forums or to look for solutions that others have made. 

**Summarizing:** use help if it is just helping you to come up with the solution by _yourself_. If you do so, at the end you will be proud of _your_ solution. ;-)

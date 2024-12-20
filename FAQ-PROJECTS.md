# FAQ - Projects - RMIT AI COSC1125/1127

This is a FAQ for the **project** assessments only.

As any FAQ page, this page is always "under construction". As we realize that some questions become common, we add them here. So, bookmark it and check it regularly, particularly when you have a doubt and you suspect it may have been answered before!

- [FAQ - Projects - RMIT AI COSC1125/1127](#faq---projects---rmit-ai-cosc11251127)
- [GENERAL](#general)
  - [In a code assignment/project, how do I make sure I do not go against academic integrity?](#in-a-code-assignmentproject-how-do-i-make-sure-i-do-not-go-against-academic-integrity)
  - [I submitted wrongly (e.g., didn't tag correctly) and is now after the due date, can you consider my submission?](#i-submitted-wrongly-eg-didnt-tag-correctly-and-is-now-after-the-due-date-can-you-consider-my-submission)
  - [Project specification says "You should code your implementation only at the locations ...." . Does this mean that we can't create our custom classes outside the provided functions?](#project-specification-says-you-should-code-your-implementation-only-at-the-locations---does-this-mean-that-we-cant-create-our-custom-classes-outside-the-provided-functions)
  - [The feedback autograder says _"Your grades are NOT yet registered."_ What should I do to register?](#the-feedback-autograder-says-your-grades-are-not-yet-registered-what-should-i-do-to-register)
  - [Should I pass all the feedback autograder tests?](#should-i-pass-all-the-feedback-autograder-tests)
  - [Why do we need to show good SE/GIT processes?](#why-do-we-need-to-show-good-segit-processes)
  - [Can I just add dummy/padding commits to have more commits?](#can-i-just-add-dummypadding-commits-to-have-more-commits)
- [GIT \& GITHUB](#git--github)
  - [Git, GitHub, what is that?](#git-github-what-is-that)
  - [Can I just use GitHub Desktop instead of command line `git`?](#can-i-just-use-github-desktop-instead-of-command-line-git)
  - [How do I submit my project solution in my GIT repository via tagging?](#how-do-i-submit-my-project-solution-in-my-git-repository-via-tagging)
  - [How do I change the submission tag if I have already tagged one commit for submission?](#how-do-i-change-the-submission-tag-if-i-have-already-tagged-one-commit-for-submission)
  - [How do I update the tags in my local repo? I get rejection with "(would clobber existing tag)" message](#how-do-i-update-the-tags-in-my-local-repo-i-get-rejection-with-would-clobber-existing-tag-message)
  - [Is a tag the same as a release in GitHub?](#is-a-tag-the-same-as-a-release-in-github)
  - [My project solution is contained in multiple commits, which do I tag?](#my-project-solution-is-contained-in-multiple-commits-which-do-i-tag)
  - [Cannot clone or push to GitHub with my password credentials?](#cannot-clone-or-push-to-github-with-my-password-credentials)
  - [I get `Permission denied (publickey).` from GitHub](#i-get-permission-denied-publickey-from-github)
  - [I have committed to the remote repo but I am not listed as a "contributor", why?](#i-have-committed-to-the-remote-repo-but-i-am-not-listed-as-a-contributor-why)
  - [Commits not correctly associated to my GitHub account, why?](#commits-not-correctly-associated-to-my-github-account-why)
  - [I made a bad commit and pushed to repo, how can I undo it?](#i-made-a-bad-commit-and-pushed-to-repo-how-can-i-undo-it)
  - [How can I check which GH username I am using for GitHub Classroom in the course?](#how-can-i-check-which-gh-username-i-am-using-for-github-classroom-in-the-course)
  - [I can't open a project in VSCode when clicking the button from GitHub](#i-cant-open-a-project-in-vscode-when-clicking-the-button-from-github)
- [PYTHON](#python)
  - [What version of Python should I use?](#what-version-of-python-should-i-use)
  - [How do I run Python 3.8 in `coreteachingXX.csit.rmit.edu.au`?](#how-do-i-run-python-38-in-coreteachingxxcsitrmiteduau)
    - [How do I install a package/module in `coreteaching` using `pip`?](#how-do-i-install-a-packagemodule-in-coreteaching-using-pip)
  - [How do I know the type of a variable in Python?](#how-do-i-know-the-type-of-a-variable-in-python)
  - [AttributeError: module 'importlib' has no attribute 'util'](#attributeerror-module-importlib-has-no-attribute-util)
  - [How do I represent infinity?](#how-do-i-represent-infinity)
  - [How do I compare the speed of my desktop/laptop with that from the cluster being used for marking?](#how-do-i-compare-the-speed-of-my-desktoplaptop-with-that-from-the-cluster-being-used-for-marking)
- [GENERAL PACMAN](#general-pacman)
  - [What is the best way to develop my solutions for the Pacman project?](#what-is-the-best-way-to-develop-my-solutions-for-the-pacman-project)
  - [How to run Pacman remotely from `coreteaching`?](#how-to-run-pacman-remotely-from-coreteaching)
  - [Python libraries and `requirements.txt` file, what are they?](#python-libraries-and-requirementstxt-file-what-are-they)
  - [How do I setup a system in Windows with Python?](#how-do-i-setup-a-system-in-windows-with-python)
  - [Can I use `problem._visited`?](#can-i-use-problem_visited)
  - [I get "`_tkinter.TclError: no display name and no $DISPLAY environment variable`" error when running in WSL or ssh](#i-get-_tkintertclerror-no-display-name-and-no-display-environment-variable-error-when-running-in-wsl-or-ssh)
  - [Cannot run Pacman due to problems with Tkinter: "`ImportError: No module named Tkinter`"](#cannot-run-pacman-due-to-problems-with-tkinter-importerror-no-module-named-tkinter)
  - [I get a blank screen when running Pacman on my Mac, why?](#i-get-a-blank-screen-when-running-pacman-on-my-mac-why)
  - [Can't fit the Pacman window in my screen, can I resize it?](#cant-fit-the-pacman-window-in-my-screen-can-i-resize-it)
  - [Cannot compile Metric-FF in MacOS](#cannot-compile-metric-ff-in-macos)
  - [I get `ModuleNotFoundError: No module named 'func_timeout'`, why?](#i-get-modulenotfounderror-no-module-named-func_timeout-why)
  - [One of the many tests is failing, how can I just run one question or even one particular test only?](#one-of-the-many-tests-is-failing-how-can-i-just-run-one-question-or-even-one-particular-test-only)
  - [My X algorithm (e.g. A\* search) works but it takes too long, what's the best way to work out why it's taking so long/work out how to optimise it?](#my-x-algorithm-eg-a-search-works-but-it-takes-too-long-whats-the-best-way-to-work-out-why-its-taking-so-longwork-out-how-to-optimise-it)
  - [How can I debug my system?](#how-can-i-debug-my-system)
  - [Can I change the pacman infrastructure at run-time?](#can-i-change-the-pacman-infrastructure-at-run-time)
  - [Can I use catch all exceptions in my code, or exceptions from the infrastructure?](#can-i-use-catch-all-exceptions-in-my-code-or-exceptions-from-the-infrastructure)
  - [Should we remove this line `util.raiseNotDefined()` before starting our code or not? What does it do?](#should-we-remove-this-line-utilraisenotdefined-before-starting-our-code-or-not-what-does-it-do)
  - [My editor shows an error trying to import pacman module](#my-editor-shows-an-error-trying-to-import-pacman-module)
  - [The autograder says `FAIL: Exception raised ...` but I am not sure which test case failed](#the-autograder-says-fail-exception-raised--but-i-am-not-sure-which-test-case-failed)
- [Project 0](#project-0)
  - [Do we have to handle edge cases? For example, for the `shopSmart` function, what should we do if a fruit is _not_ present in one of the shops?](#do-we-have-to-handle-edge-cases-for-example-for-the-shopsmart-function-what-should-we-do-if-a-fruit-is-not-present-in-one-of-the-shops)
  - [Does the reference to 'pounds' in buyLotsOfFruit.py refer to weight (lb) or cost (£)?](#does-the-reference-to-pounds-in-buylotsoffruitpy-refer-to-weight-lb-or-cost-£)
- [Project 1](#project-1)
  - [Do we need to do all the "`*** YOUR CODE HERE ***`" method?](#do-we-need-to-do-all-the--your-code-here--method)
  - [Can I import standard libraries?](#can-i-import-standard-libraries)
  - [What actions should I return in the search algorithms?](#what-actions-should-i-return-in-the-search-algorithms)
  - [How can I represent a plan with no actions?](#how-can-i-represent-a-plan-with-no-actions)
  - [What counts as an expansion? I am getting too many expansions....](#what-counts-as-an-expansion-i-am-getting-too-many-expansions)
  - [My solution works manually for `tinaMaze` but the authograder fails. The state format used in the autogarders tests are different from the Pacman game's in `tinaMaze`. What happens here?](#my-solution-works-manually-for-tinamaze-but-the-authograder-fails-the-state-format-used-in-the-autogarders-tests-are-different-from-the-pacman-games-in-tinamaze-what-happens-here)
  - [In Q7, can I take a heuristic from elsewhere (e.g., Google) and implement it?](#in-q7-can-i-take-a-heuristic-from-elsewhere-eg-google-and-implement-it)
  - [In Q7, what timeout will be used? How do I know what timeout should I use?](#in-q7-what-timeout-will-be-used-how-do-i-know-what-timeout-should-i-use)
  - [Are we allowed to use `mazeDistance` (or a modified version) when calculating our heuristic?](#are-we-allowed-to-use-mazedistance-or-a-modified-version-when-calculating-our-heuristic)
  - [Can we create a new BFS for the part 5? My implementation doesn't fit with my new state representation!](#can-we-create-a-new-bfs-for-the-part-5-my-implementation-doesnt-fit-with-my-new-state-representation)
  - [Break-points do not work on `search.py`, why?](#break-points-do-not-work-on-searchpy-why)
  - [In the feedback autograder, what does `expanded_states` means?](#in-the-feedback-autograder-what-does-expanded_states-means)
  - [What we should return for the failure case, ie. when no path can be found?](#what-we-should-return-for-the-failure-case-ie-when-no-path-can-be-found)
  - [For Q9 cycle checking, should we check only a few levels, or all the way up to the root node?](#for-q9-cycle-checking-should-we-check-only-a-few-levels-or-all-the-way-up-to-the-root-node)
  - [In Q6 or Q7 I am getting `FAIL: inconsistent heuristic path` for a test case, what does this mean?](#in-q6-or-q7-i-am-getting-fail-inconsistent-heuristic-path-for-a-test-case-what-does-this-mean)
- [Project 2](#project-2)
  - [Inconsistent depth in minimax project 2, Q2 and careful use of `__init__`](#inconsistent-depth-in-minimax-project-2-q2-and-careful-use-of-__init__)
  - [Can we apply a "magic number" such as -9999 in our evaluation functions, as part of our logic not simply an arbitrary "return -9999"?](#can-we-apply-a-magic-number-such-as--9999-in-our-evaluation-functions-as-part-of-our-logic-not-simply-an-arbitrary-return--9999)
  - [In Q4, what does it mean an adversary which chooses amongst their `getLegalActions` uniformly at random?](#in-q4-what-does-it-mean-an-adversary-which-chooses-amongst-their-getlegalactions-uniformly-at-random)
  - [The results of the feedback autograder with graphics and without graphics are very different! My system works without graphics but times out with graphics and I lose all games, why?](#the-results-of-the-feedback-autograder-with-graphics-and-without-graphics-are-very-different-my-system-works-without-graphics-but-times-out-with-graphics-and-i-lose-all-games-why)
  - [When I run the autograder I get the message _"has not SIGALRM"_, why?](#when-i-run-the-autograder-i-get-the-message-has-not-sigalrm-why)
  - [What is a reasonable time for Question 5?](#what-is-a-reasonable-time-for-question-5)
  - [Is there a way to run the evaluation function in Question 5 in harder setting or with more ghosts?](#is-there-a-way-to-run-the-evaluation-function-in-question-5-in-harder-setting-or-with-more-ghosts)
  - [Unlike in P1, we are not given explicit pseudocode, can we still follow the book?](#unlike-in-p1-we-are-not-given-explicit-pseudocode-can-we-still-follow-the-book)
  - [Can I reuse code from P1 in my heuristic evaluation function (e.g. copy my A* search over?)](#can-i-reuse-code-from-p1-in-my-heuristic-evaluation-function-eg-copy-my-a-search-over)
  - [Autograder is passing Q1, but the scores from the games are negative, is this ok?](#autograder-is-passing-q1-but-the-scores-from-the-games-are-negative-is-this-ok)
- [Project 3](#project-3)
  - [I want to get a head start and learn prolog now! How can I do it?](#i-want-to-get-a-head-start-and-learn-prolog-now-how-can-i-do-it)
  - [GitHub is telling me all checks have failed, but some tests are passing on my machine, is this a problem?](#github-is-telling-me-all-checks-have-failed-but-some-tests-are-passing-on-my-machine-is-this-a-problem)
  - [GitHub error on push `The following actions use a deprecated Node.js ...`](#github-error-on-push-the-following-actions-use-a-deprecated-nodejs)
  - [Is it ok to change the parameter structure of the predicates we are told to implement?](#is-it-ok-to-change-the-parameter-structure-of-the-predicates-we-are-told-to-implement)
  - [Is it ok to define multiple versions of the predicates (helpful for base and edge cases)?](#is-it-ok-to-define-multiple-versions-of-the-predicates-helpful-for-base-and-edge-cases)
  - [Is it ok to define helper functions?](#is-it-ok-to-define-helper-functions)
  - [My solution prints false when the example doesn't, or warning: `Test tools_for_items_2: Test succeeded with choicepoint`](#my-solution-prints-false-when-the-example-doesnt-or-warning-test-tools_for_items_2-test-succeeded-with-choicepoint)
  - [Best way to check empty list in Prolog](#best-way-to-check-empty-list-in-prolog)
  - [Do we need to handle cyclic dependencies?](#do-we-need-to-handle-cyclic-dependencies)
  - [What do the question marks mean in the predicate: `tool_for_item(?Item, ?Tool)`?](#what-do-the-question-marks-mean-in-the-predicate-tool_for_itemitem-tool)
  - [I can't see the full output in prolog, I am getting dots instead indicating it continues. How can I see everything?](#i-cant-see-the-full-output-in-prolog-i-am-getting-dots-instead-indicating-it-continues-how-can-i-see-everything)
- [Project 4](#project-4)
  - [What are 'Noise' and 'LivingReward' in Q3?](#what-are-noise-and-livingreward-in-q3)
  - [How should we come up with values for Q3? Do we just guess? Do we have to explain it?](#how-should-we-come-up-with-values-for-q3-do-we-just-guess-do-we-have-to-explain-it)
  - [What do I need to do for Q7? The autograder passes without any new code.](#what-do-i-need-to-do-for-q7-the-autograder-passes-without-any-new-code)
  - [The textbook algorithm for Value Iteration takes $\epsilon$ as a parameter, where is this in the project code?](#the-textbook-algorithm-for-value-iteration-takes--as-a-parameter-where-is-this-in-the-project-code)
  

-------------------------

# GENERAL

## In a code assignment/project, how do I make sure I do not go against academic integrity?

Check the [answer to this key question here](../AI23-DOC.git/CODE-INTEGRITY.md)

## I submitted wrongly (e.g., didn't tag correctly) and is now after the due date, can you consider my submission?

We will not fix any submission and it is your responsibility to do it correctly.

However, the nice thing about git-based projects/assessments is that we can rely on commits. So, if you have submitted your tag incorrectly (did not tag it at all, tagged with different name or different capital letters), then please fix your submission by tagging the specific commit you want me to (re)mark and let us know you did so in the corresponding PR of your repo (no email, no forum). 

Note we will of course use the timestamp of the commit itself, not of when it was tagged. This means that if the commit was done before the deadline, then all good!! Isn't this cool?

## Project specification says "You should code your implementation only at the locations ...." . Does this mean that we can't create our custom classes outside the provided functions?

You can create some help functions or classes, but **always** in the allowed files. Any other change in any other file will be totally ignored.

If you want to create custom classes and functions, you can also nest them inside the location where you read `***YOUR CODE HERE***`. See [this link](https://www.datacamp.com/community/tutorials/inner-classes-python) and [this link](https://www.programiz.com/python-programming/closure#:~:text=A%20function%20defined%20inside%20another,in%20order%20to%20modify%20them) for more info.

## The feedback autograder says _"Your grades are NOT yet registered."_ What should I do to register?

The autograder is some immediate **feedback** for you, but it is not the final grading we do as teaching staff.

So, while the automarker is a useful indication of your performance, it may not represent the ultimate mark. We reserve the right to run more tests, inspect your code and repo manually, run similarity software for integrity checks (this year via [Codequiry](https://codequiry.com/)), and arrange for a face-to-face meeting for a discussion and demo of your solution if needed.

After submission deadline we will mark them all and provide you with the results.

## Should I pass all the feedback autograder tests?

Well, if you want to have a chance to get full marks _yes_.

Basically, the feedback autograder given is the _bare minimum_ and it is meant to provide you with some help in you development. In fact, even if your solution does meet every feedback test case given, it still does not necessarily mean it is perfect, as we may run additional tests when we actually grade the submission. Again, the autograder is an invaluable feedback tool for development and is the bare minimum, but more will be asked. You are encourage to extend it with your own tests and to perform your own extended efficiency evaluation when appropriate.

We are aware that it can be a bit unforgiving to work with the automated test harness, but often your understanding of the underlying algorithms are greatly improved when you need to dig into particular corner cases, so it's time well spent.

As recognised by students, the autograder is indeed a fantastic feedback before submission for you. It is the minimum expected and you have it right from the start, so use it!

## Why do we need to show good SE/GIT processes?

It is a fair question: _why don't we just care about the AI algorithm and that's it?_

There are are least three main reasons to include SE and version control practices as part of the work and assessments of the course:

- We want to see the _**process**_ towards your solution, not just the solution(s) to a question. We want to be able to see _evidence of student workings towards_ the final solution.
    - This is **analogous to when we do Maths**: we do not want to see just the final answer, but also HOW you got to that answer.
    - This process will include your intermediate and alternative solutions, your partial solutions, your bugs and fixes, your optimisations, your thought process, etc.
- **Good development of AI techniques** (and software in general) is also super important today, and a place for learning. It is _the way AI software and solutions are developed these days_, the state-of-the-art. Hence, good SE practices, and particularly version control, is part of the overall training we promote in our courses, particularly in advanced courses.
- Version Control contributes to CLO 5 (on develop _adequate_ AI solutions for problems) as well as CLO 6 (_communicate_ with the language of the field). Version control is not only the adequate way to develop complex software but also a way to communicate to others your work and solutions.

Note that the number of commits is not per se "the issue," that is, it is not about counting and "the more the better." Lots of dummy, non-meaningful, commits is also very poor. However, a very low number of atomic meaningful commits is a proxy that could **signal qualitative problems** in terms of good development process. That is why we expect students to critically judge what is a good history and what is a poor one, which one show evidence of sustainable work and which one does not. The good healthy history should come as a natural consequence of the work done. It would be very poor educationally to say "16 commits," because this is a qualitative criteria first.

Finally, the expectations on this have been very clearly stated from Project 0, including stating that "bulk commits will be heavily penalised" as they show no evidence of student's working to the solution and are at odds with state-of-the-art AI development. Besides the issue being explicitly mentioned in project specifications, lectorials, slides, forum and FAQ, we provided a clear guide on each dimension and clear examples of what are good development histories in GIT; see [HERE](SE-PRACTICES.md).

Hope this puts some context and rationale to the issue, and serves as a good learning opportunity!

## Can I just add dummy/padding commits to have more commits?

**No!**

That will not only show very poor SE practices (because dummy commits are not meaningful commits), but most importantly it may be deemed as a case of "_dishonest behavior to get an unfair advantage_", which is against the course Honours Code and can be a serious offense. One thing is to have poor SE practices, another thing is to attempt to cheat, so that should be out of the question! :-)

------------------------------
# GIT & GITHUB

## Git, GitHub, what is that?

We will use proper (git) version control in all our programming projects. This is totally standard practice in the industry and you would have seen that in previous courses (SEF and SEPT at least). Said so, if you want to refresh or have a quick intro to it, here are two resources I found useful:

- [30' video on Git & GitHub](https://youtu.be/jG4Vs81kMlc).
- [GitHub Guides](https://guides.github.com/).
- [Git \& GitHub Tutorial & Reference @ Javatpoint](https://www.javatpoint.com/git).

There are lots more good resources on the web of course!

## Can I just use GitHub Desktop instead of command line `git`?

You can use it, as long as you are also able to resort to command line `git` when needed.

GitHub Desktop, or any other programming tool like a text editor/IDE, package manager, etc, have strengths and limitations. While using GitHub Desktop is not inherently bad, as long as it is fit for your purpose and provides an efficient workflow, there is value in having an understanding how the tools work, because that will help you when they fail or you reach their limits. But as long as you are confident that you could understand the underlying details if you needed to, all good! 👍

Now, if you are using GitHub Desktop just because you do not know how to use git command line, then that is ineed not good enough (both in terms of skills and attitude) for a student taking this course, and a CS/IT student overall anwyays. You are expected to be able to know git more than its high-level tools, and to learn whatever gaps you have. 😉

Critically, you will not get help from staff about how to use GitHub Desktop, since we (or at least most of us) don't use it. 🤦


## How do I submit my project solution in my GIT repository via tagging?

You submit by **tagging the _exact_ commit that you want to submit and be marked**, using the exact name given in the assignment specification. We will ONLY marked tagged submissions and will ONLY mark the tagged commit. Students can have many commits, and branches, even commits after the deadline. We will mark ONLY what you submit.

Of course we do not have access to your local machine, so the tag has to be created locally or then _pushed_ into GitHub remote repo (see below for several guides). Your tag has to show under `tags`, for example:

![google-form](img/tags-github-gui.png)

Observe that a tag `submission` is:

- NOT the same as a tag called "`Submission`" (i.e., tags are case-sensitive);
- NOT the same as a _branch_ called "`submission`";
- NOT the same as a _commit message_ "`submission`"; and
- NOT the same as a _release_ called "`submission`".

A tag is a specific point in the repository history, the point you want to be used for marking. A branch, a comment, and a release are different things.

While you can tag from your IDE (e.g., VS Code) you can always resort to command line to first create the tag in your local repo and then push it to the remote:

```shell
$ git tag -a submission <hash of commit to tag>
$ git push origin submission
```

By `<hash of commit to tag>`, we mean the 6-8 character hexadecimal string which uniquely identifies a commit.
Check the remote has the tag where you wanted and that it also contains all the commits you did towards the tag!

> [!IMPORTANT]
>
> Before pushing your tag to the remote repo, make sure all the commits you did have already been pushed to the remote too. Check that in the GitHub remote. It is wrong to push just the tag without pushing the actual commits, as it will yield a tag not belonging to any branch history:
>
> ![](img/tag-no-commits.png)


Note that _a tag name can only be used once_, so if you already have a tag `submission` and want to use that tag name on another commit (e.g., you have a better, more recent, commit for your solution), you first need to delete the existing tag; see the next question for that. :-)

- For basic information on tagging, check [here](https://git-scm.com/book/en/v2/Git-Basics-Tagging).
- To create, push, and view tags in GitHub Desktop, check [here](https://docs.github.com/en/desktop/contributing-to-projects/managing-tags).
- To tag via command line or via GitHub web interface, check [here](https://stackoverflow.com/questions/18216991/create-a-tag-in-a-github-repository).

Note that the timestamp of the _commit_ is the submission date.

## How do I change the submission tag if I have already tagged one commit for submission?

This will happen when you realize you have a better version to submit than the one you submitted/tagged before. To do that, you need to first _delete_ the existing tag from both your local repo and from the server:

```shell
$ git tag --delete <tagname>  # first delete tag in the local repo
$ git push origin :refs/tags/<tagname>  # then delete remote tag
```

It is important to use `:refs/tags` when deleting the remote tag, as otherwise you may delete the branch with the same name! The empty string to the left of the colon causes the remote reference to be deleted!

Once the tag has been fully deleted, so you can re-use it on another commit!

See this as well on how to _rename_ an existing tag:

![google-form](img/how-to-rename-tag.png)

More information on how to delete git tags [here](https://devconnected.com/how-to-delete-local-and-remote-tags-on-git/).

## How do I update the tags in my local repo? I get rejection with "(would clobber existing tag)" message

To fetch the tags in the remote (e.g., tags pushed by other collaborators), you can do:

```shell
$ git fetch --all --tags -f
```

This will fetch all the changes from the remote, but also all the tags. The `-f` option will replace an existing tag (e.g., `submission`) with the one in the remote, if any (instead of failing). This could come very handy when different collaborators tag and re-tag commits as they incrementally work on a solution.

## Is a tag the same as a release in GitHub?

No, a _tag_ is a _git concept_, whereas a `Release` is something about GitHub, beyond git itself. So, they are not synonymous.

A tag is a _pointer_ to a specific commit, that's all, you basically give a name to a specific commit. This is what we use to mark the commit that is meant to be submitted for marking.

## My project solution is contained in multiple commits, which do I tag?
The last one. 
I think the confusion here is because there are two potentially different things you can mean with the same word commit.
You are thinking of commit as a set of changes to files - so the commit itself is only made up of the edits you have made since the last commit.
We are thinking of a commit as a snapshot of the entire repository at a point in time, which shows exactly what all the files looked like in the repo in their entirety.

A commit is both things! (I will spare you links to documentation to prove it). 
As a result, when you commit your final changes to the assignment (even if it is just changing your name in a readme file), and then you tag that commit, we can see all of the files that exist in the repo after you have completed everything. No need to 'recommit' things which you have done before.

To make you comfortable with this, browse around the GitHub page for your project repo. When you make a tag, you should be able to see a link to it, and even download the repo at that tag as a zip file. If you unzip it, you will see the entire repo. 

## Cannot clone or push to GitHub with my password credentials?

As [per August 12th, 2021 GitHub post](https://github.blog/changelog/2021-08-12-git-password-authentication-is-shutting-down/), GitHub is not no longer accepting account passwords when authenticating Git operations, like cloning private repos or pushing changes. You should use **token-based authentication**, such as  personal access, OAuth, SSH Key, or GitHub App installation token.

So, if you were still using a password to authenticate your GitHub.com operations (something never recommended anyways if you are doing development), you must start using a [personal access token](https://docs.github.com/en/github/authenticating-to-github/keeping-your-account-and-data-secure/creating-a-personal-access-token) by August 13, 2021 via HTTPS (recommended) or [SSH key](https://docs.github.com/en/github/authenticating-to-github/connecting-to-github-with-ssh) to start using a personal access token to avoid disruption.

For example, you can set-up your remote as follows (after you generated your token in GitHub):

```shell
$ git remote set-url origin https://<token>@github.com/<username>/<repo>
```

As explained [here](https://www.sobyte.net/post/2021-08/github-deprecates-passwords-for-git-operations/), tokens offer many advantages over password-based authentication:

* **Unique:** tokens are specific to GitHub and can be generated on a per-use or per-device basis.
* **Revocable:** tokens can be individually revoked at any time without the need to update unaffected credentials.
* **Limited:** tokens can be narrowed to allow only the access required by the use case.
* **Random:** tokens are not subject to dictionary types or brute force attempts that might be made with simpler passwords that users need to remember or enter periodically.

## I get `Permission denied (publickey).` from GitHub

If yo get this error

```shell
git@github.com: Permission denied (publickey).
fatal: Could not read from remote repository.
```

it most probably mean you have not correctly set-up your ssh keys into GitHub. GitHub needs your ssh public key to know it's you who is trying to access the repo. Please check [here](https://docs.github.com/en/authentication/troubleshooting-ssh/error-permission-denied-publickey).

Setting up GitHub to access with token or ssh is fundamental to have a productive environment, as you will be pushing and pulling from GitHub a lot! :-)

## I have committed to the remote repo but I am not listed as a "contributor", why?

The two main reasons may be:

1. Your commit is in a branch and has not yet made it to the default (master/main) branch, therefore you did not technically contribute (yet).
2. Your local Git commit email isn't connected to your account; [connect it](https://docs.github.com/en/github/setting-up-and-managing-your-github-user-account/managing-email-preferences/setting-your-commit-email-address)!

Read [this GitHub page](https://docs.github.com/en/github/setting-up-and-managing-your-github-profile/managing-contribution-graphs-on-your-profile/why-are-my-contributions-not-showing-up-on-my-profile#common-reasons-that-contributions-are-not-counted) to understand more about why your commit is not yet counting as contributions.

## Commits not correctly associated to my GitHub account, why?

Please [check this](https://docs.github.com/en/github/committing-changes-to-your-project/troubleshooting-commits/why-are-my-commits-linked-to-the-wrong-user) and fix it so we can know the commit was *yous*. Otherwise we may get your contributions wrong and risk getting lower marks or delaying your marking.

Note that when you [set your email address in git in your machine](https://docs.github.com/en/account-and-profile/setting-up-and-managing-your-personal-account-on-github/managing-email-preferences/setting-your-commit-email-address#setting-your-commit-email-address-in-git) you can do it globally, or per repo. The latter would be useful if you are using different GH usernames for different projects/repos (e.g., for different courses, or personal projects).

## I made a bad commit and pushed to repo, how can I undo it?

You should use `git revert`. That is, if you  pushed your changes and you now want to go back to the previous version, use this (assuming you are working on the `main` branch):

```shell
$ git revert HEAD~1
$ git push origin main
```

This states that you want to revert the changes to `HEAD` by `1` commit (the last commit), make a new commit that undoes those changes, and then push this new commit to the origin branch, in this case the `main` branch. Of course you can imagine how to undo back more than 1 commit, right? ;-)

Read more about `git revert` [here](https://www.atlassian.com/git/tutorials/undoing-changes/git-revert).

## How can I check which GH username I am using for GitHub Classroom in the course?

The GitHub username you selected is in the name of all of the projects you clone. (e.g. if the repo is called `project-1-search-<username>`, then you used GH `username` account). This is the account with which you should make commits with so we can link them to you through classrooms. You must then have your GIT configuration to commit with such user so that your commits are counted as yours. See [this question](#i-have-committed-to-the-remote-repo-but-i-am-not-listed-as-a-contributor-why) as well.

# I can't open a project in VSCode when clicking the button from GitHub

This is often due to a space in a file path on your machine (generally for Windows users), but might have other causes. This button relies on a VSCode extension that is deprecated, so may not be reliable. We strongly encourage all students to clone the repository locally on their machine, and work from there. 

------------------------------
# PYTHON

## What version of Python should I use?

All projects run on **Python 3.9+**, so your code must be written for such a version. We use Python 3.10. Note that Python 3.8 is [ending its support these days](https://devguide.python.org/versions/).

Some Linux distributions come with both `python2` and `python3` installed but default to `python2` for the python command. In this case, you should use the `python3` command in place of python to explicitly use version 3.x.

Additionally, in order to render the game, the homework projects require the Python module `tkinter` to be installed. You can follow the [official docs](https://tkdocs.com/tutorial/install.html) to get `tkinter` on your platform if it is not installed already. If you are using Linux, many distributions have packaged `tkinter` for easy install and you should use the package manager to install it. The package name is `python3-tk` for Debian/Ubuntu, `python3-tkinter` for RHEL/Fedora and `tk` for Manjaro/Arch.

There is no problem **having more than one Python version installed in your machine**, you just need to be careful your code is using the right one. You can use Python Package and Environment Managers, such as [Conda](https://www.freecodecamp.org/news/why-you-need-python-environments-and-how-to-manage-them-with-conda-85f155f4353c/) or [miniconda](https://conda.io/miniconda.html) environments, or an environment with [PIP+virtualenv](https://uoa-eresearch.github.io/eresearch-cookbook/recipe/2014/11/26/python-virtual-env/).

## How do I run Python 3.8 in `coreteachingXX.csit.rmit.edu.au`?

We do not recommend using those servers, they are fairly out-of-date and you have very little control over them (e.g., what you can install). These days the best option is to use your own machine/laptop.

The default Python in these servers is 2.7! 🤦 However, you can activate 3.6 and 3.6 using `scl`:

```bash
[eXXXXX@csitprdap01 ~]$ scl enable rh-python38 bash
[eXXXXX@csitprdap01 ~]$ python --version
Python 3.8.18
[eXXXXX@csitprdap01 ~]$ python
Python 3.8.18 (default, Oct 24 2023, 08:42:25)
[GCC 9.1.1 20190605 (Red Hat 9.1.1-2)] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>>
```


### How do I install a package/module in `coreteaching` using `pip`?

Use option `--user` as you cannot do system-wide install:

```shell
[eXXXX@csitprdap01 ~]$ pip install pytz --user
WARNING: pip is being invoked by an old script wrapper. This will fail in a future version of pip.
Please see https://github.com/pypa/pip/issues/5599 for advice on fixing the underlying issue.
To avoid this problem you can invoke Python with '-m pip' instead of running pip directly.
Collecting pytz
  Using cached pytz-2022.1-py2.py3-none-any.whl (503 kB)
Installing collected packages: pytz
Successfully installed pytz-2022.1
```

## How do I know the type of a variable in Python?

Check this video to know how to print the type of a variable in Python:

[![Alt text](https://img.youtube.com/vi/iROZLaQGy4s/0.jpg)](https://www.youtube.com/watch?v=iROZLaQGy4s)

## AttributeError: module 'importlib' has no attribute 'util'

Some students reported that running `python capture.py` gives them the following errors:

```shell
Traceback (most recent call last):
  File "capture.py", line 1127, in <module>
    options = readCommand( sys.argv[1:] ) # Get game components based on input
  File "capture.py", line 902, in readCommand
    redAgents = loadAgents(True, options.red, nokeyboard, redArgs)
  File "capture.py", line 978, in loadAgents
    spec = importlib.util.spec_from_loader(moduleName, loader)
AttributeError: module 'importlib' has no attribute 'util'
```

Changing `import importlib` with `import importlib.util` seems to fix the problem.

We are still investigating this issue as it seems to work well in our set-up. This seems to be related to the fact that ["importing a package does not automatically load its submodules"](https://stackoverflow.com/questions/65028261/attributeerror-module-importlib-has-no-attribute-util-ii) but we are unclear why sometimes it does work! A quick search also brings [this post](https://stackoverflow.com/questions/39660934/error-when-using-importlib-util-to-check-for-library) which may be

## How do I represent infinity?

The best way is to use [`math.inf`](https://docs.python.org/3/library/math.html#math.inf). Python can handle arbitrarily large numbers, and so `math.inf` is both correct and also meaningful for the reader.

**Note:** avoid using `sys.maxsize`; you can check what happens if you do `sys.maxsize < sys.maxsize*2`. :-)

## How do I compare the speed of my desktop/laptop with that from the cluster being used for marking?

In general the cluster is not very fast, hence it won't be a surprise if your laptop runs faster.

You can compare the relative speed of your machine against the cluster using [python-speed](https://github.com/vprelovac/python-speed).

This is what I get in the cluster:

```shell
$ python bench.py
python-speed v1.3 using python v3.10.12
string/mem: 2187.5 ms
pi calc/math: 2867.82 ms
regex: 3132.5 ms
fibonnaci/stack:  1904.6 ms
multiprocess: 1297.76 ms

total:  11390.18 ms (lower is better)
```

And this is what I get from my laptop:

```shell
$ python bench.py
python-speed v1.3 using python v3.10.12
string/mem: 1126.62 ms
pi calc/math: 2231.34 ms
regex: 1877.54 ms
fibonnaci/stack:  1250.05 ms
multiprocess: 509.13 ms

total:  6994.68 ms (lower is better)
```

As you can see my laptop is ~2x faster than the cluster machine! So, _how fast is your laptop_?

------------------------------
# GENERAL PACMAN

## What is the best way to develop my solutions for the Pacman project?

We highly recommend developing your solutions in your local machine, that is, your laptop or desktop. Even more, if you are running Linux locally, 99.99% sure your code will ran in another Linux install. If you are using Windows, you may want to consider installing a Linux virtual machine with Virtualbox.

Secondly, you should use a modern IDE. We recommend Visual Studio Code, as it runs in any platform and has plugins for all the languages we will be using. It also has great git integration plugins and much more.

Also, all development should be done using high-quality version control processes. The course will use GitHub and GitHub Classroom. All development should happen there. Remember NOT to make your solutions public, as this will violate the course plagiarism code AND also break the will of the original creators of the wonderful project.

So, (local machine + VSCode (or other IDE) + git) will make the development much faster and higher-quality.

## How to run Pacman remotely from `coreteaching`?

If you do not care about the graphics (e.g., for grading), then try using `--textGraphics` or even `--quietTextGraphics`. In most cases you will use `coreteaching` machines just to test that the autograder works well. The autograder does not need any graphical interface so it should work properly.

If you do want the display, then you need to do X forwarding when you connect via ssh. If you are in Linux/Unix this is easy, just do `-X` and `-Y` when you ssh; for example:

```shell
$ ssh -X -Y username@coreteaching01.csit.rmit.edu.au
```

If you use Windows, then you need an X server running and set your ssh client (e.g., Putty) with X forwarding. For example, check [this page](https://superuser.com/questions/119792/how-to-use-x11-forwarding-with-putty) or this video:

[![Alt text](https://img.youtube.com/vi/vwZXhTykSis/0.jpg)](https://www.youtube.com/watch?v=vwZXhTykSis)

Said so, for development, we strongly suggest to clone your repo locally on your machine and work there (e.g., using PyCharm, Visual Code Studio, or even ECLIPSE).

## Python libraries and `requirements.txt` file, what are they?

The file `requirements.txt` should have the libraries that are required, you can get these modules running:

```shell
$ pip install -r requirements.txt
```

You will see in some other questions in this FAQ that some errors are because the system is missing some library (like `tk` for the graphical display).

## How do I setup a system in Windows with Python?

Although we will assume you are able to install and get Python running in your machine, there are plenty of videos on that on the web. For example:

[![Alt text](https://img.youtube.com/vi/oHOiqFs_x8Y/0.jpg)](https://www.youtube.com/watch?v=oHOiqFs_x8Y)

## Can I use `problem._visited`?

Under Python convention, single underscore before a name (e.g., `_visited`) denotes private data, and hence it is good practice not to rely on such data. Check [this post](https://shahriar.svbtle.com/underscores-in-python) for example. Note that such private data can change without notice, it may not be available anymore, it may not be available under other interfaces, etc. So....

## I get "`_tkinter.TclError: no display name and no $DISPLAY environment variable`" error when running in WSL or ssh

If you do not care about the graphics, then try using `-t` (or `--textGraphics`) or even `-q` (or `--quietTextGraphics`).

If you do want the display, then you need to do X forwarding when you connect via ssh. If you are in Linux/Unix this is easy, just do `-X` and `-Y` when you ssh (e.g., `ssh -X -Y server`).

If you use Windows, then you need an X server running and set your ssh client (e.g., Putty) with X forwarding. For example, check [this page](https://superuser.com/questions/119792/how-to-use-x11-forwarding-with-putty) and [this video](https://www.youtube.com/watch?v=vwZXhTykSis).

Also, if you are using Windows hooked up into Linux (WSL or WSL2), you need to properly resolve the IP Address seen by Linux. For example, under Ubuntu bash, add this to your `~/.bashrc`:

```shell
export DISPLAY=$(cat /etc/resolv.conf | grep nameserver | awk '{print $2}'):0
```

Then install the [VCXSRV](https://sourceforge.net/projects/vcxsrv/files/vcxsrv/) X-server. Run xLaunch and "Disable access control". And add a new inbound rule in Windows Firewall for TCP Port 6000.  Use the ssh command as above.

As you can see, all these can be too complicated for no benefit. For development, **we strongly suggest** to clone your repo locally on your machine and work there (e.g., using PyCharm, Visual Code Studio).

## Cannot run Pacman due to problems with Tkinter: "`ImportError: No module named Tkinter`"

Install Tkinter in your system. In general this is easy to do via:

```shell
$ pip install tk
```

Now it should be installed, so you should not get this error. But please try the code below, it should not trigger any error:

```shell
❯ python
Python 3.10.12 (main, Mar 22 2024, 16:50:05) [GCC 11.4.0] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> import tkinter
>>>
```

If you are running `conda`:

```bash
$ conda install tk
```


## I get a blank screen when running Pacman on my Mac, why?

If you get something like this on your Mac:

![Blank screen on Mac](img/tkinter-mac-python2.jpg)

This may be due to using Python 2.7. Any Mac users, make sure to run `python3 pacman.py` (or otherwise ensure you are using Python 3, not 2.x).
Another cause seems to be related to using the wrong virtual environment. From a student:
"To resolve this, I switched to using the Python 3.9 virtual environment as the interpreter, which corrected the issues.
I initially tried using Pyenv with Python 3.9, but it still didn't work. Then I switched to Conda, and surprisingly, everything started working fine."

## Can't fit the Pacman window in my screen, can I resize it?

The Pacman windows cannot be resized once open. However, you can use the option `-z <float>` (or `--zoom <float>`) to scale the window. For example, using `-z 0.5` will scale down the window by half. Using this option you should be able to fit the entire window in the screen.

## Cannot compile Metric-FF in MacOS

Some Mac users have reported this error when compiling [Metric-FF](https://fai.cs.uni-saarland.de/hoffmann/metric-ff.html) planner:

![bad-graphics](img/ff-compile-mac.png)

The problem seems to be that the default `gcc` in Mac is set to be `clang`. So, you first neeed to install standard `gcc` on using command `brew install gcc@7`  (must use version 7, newest version 10 won't work) and instead of just `make`, you need to run:

```bash
make CC=/usr/local/bin/gcc-7
```

Thanks Banhao from AI'20!

## I get `ModuleNotFoundError: No module named 'func_timeout'`, why?

This should be easy to troubleshoot, but there are certain Python packages/modules that are needed:

```shell
$ pip install func_timeout
$ pip install pytz
```

## One of the many tests is failing, how can I just run one question or even one particular test only?

Use the `-q n` option for running just one question (e.g., `-q q3` to run Question 3 only) or `-t` to run only a specific test (e.g., `-t test_cases/q1/graph_bfs_vs_dfs`).

## My X algorithm (e.g. A* search) works but it takes too long, what's the best way to work out why it's taking so long/work out how to optimise it?

Fundamentally there are two ways of approaching this, empirically or theoretically.

Empirically you can profile your code and see which sections are taking the longest. If you have a particular section that you suspect might be the issue, you can use the time module to check manually. However probably the better way is to use pythons inbuilt `cprofile` tool. This works well, especially when paired with [Snakeviz](https://stackoverflow.com/a/49173782). There is also
[line_profiler](https://github.com/pyutils/line_profiler) which profiles line by line showing line time, total line time and number of calls.

Theoretically, you can use your algorithms and analysis skills to try to figure out the time complexity of your algorithm. If your code matches the book, it should have a similar time complexity, but you may want to dig a bit deeper into each individual line of code. What is the time complexity of popping from a priority queue in python? What about a list? What about adding a node to the frontier, or visited data structure?

In general, before spending a lot of time doing experimental analysis, look at your implementation conceptually in a very, I repeat, _very_, critical way and perform the (theoretical) analysis of it. Think where the problem could be and whether you can suspect of something that is not well done. It's like being a detective, and good detectives are critical and meticulous!

## How can I debug my system?

While you may want to do some print outs here and there, eventually using a debugger is the way to go. Check [this video](https://www.youtube.com/watch?v=w8QHoVam1-I) for a quick guide to debugging python in VSCode (you can do similar things in PyCharm or other editors as well). This is far more flexible and reliable than print messages. :-) 

To make life easy for yourself, you will want to create a debugging configuration in VSCode which runs the autograder file, regardless of which file you have open. You will also want to pass in the arguments `-q q1` to run only the first question (or whichever you are interested in). You can accomplish this by adding the following text to the `launch.json` file which stores all the debug configurations:
```json
      {
          "name": "Python Debugger: autograder",
          "type": "debugpy",
          "request": "launch",
          "program": "autograder.py",
          "console": "integratedTerminal",
          "args": [
              "-q",
              "q1"
          ]
      }
```

## Can I change the pacman infrastructure at run-time?

**Absolutely no!** You should never tamper with the Pacman codebase infrastructure in any project, neither at the source code level nor at run-time. That is not allowed for any project: your agent systems should alter anything in the infrastructure, even at runt-time, unless you have been given explicit permission in writing.

As a general rule, reading properties of the infrastructure is OK and you will need to do so indeed. But **modifying the infrastructure at run-time in any way is not OK**. First it is poor technical approach to rely on that. Second, it may _unfairly_ give you an advantage, and in the contest project, may even affect other teams; for example by making them fail!

For example, doing this in the contest project:

```python
Actions._directions.pop('Stop', None)
```

will delete the action `Stop` from the set of legal directions. That is of course NOT allowed as you are tampering with the infrastructure, not just with your own code. Instead, you should do something like this:

```python
# Get legal actions from the agent and remove "Stop"
actions = gameState.getLegalActions(self.captureAgent.index)
actions.remove(Directions.STOP)
```

Here is another example that interferes badly with the infrastructure:

```python
agent.configuration.direction = "North"
```

This is setting a property of the agent: that is done by the infrastructure as part of the simulation and you should not interfere.

Even a more serious one would be to override `makeObservation` or any other function or class in the infrastructure. Never ever do that.

In fact, tampering with the infrastructure could be considered as dishonest behavior to get an unfair advantage. If you are in doubt, then ASK, never assume. Not asking before tampering with the codebase is in fact very worrying, even more for an advance course like AI.

We have specialized checks to test that the infrastructure is kept unchanged.

So please, remove absolutely every code that modifies, changes, or alter, even minimally, any part of the infrastructure and make sure you play _fair_ and don't make Pacman cry...

## Can I use catch all exceptions in my code, or exceptions from the infrastructure?

**Absolutely no!** It is first a very [bad practice](https://www.learnpython.dev/03-intermediate-python/40-exceptions/70-best-practices/#:~:text=Catching%20BaseException%20is%20a%20really,Don't%20do%20it.), as stated in PEP-8 and so many pages around:

> When catching exceptions, mention specific exceptions whenever possible instead of using a bare `except:` clause.

So, instead of doing:

```python
try:
    import platform_specific_module
except:
    platform_specific_module = None
```

you should instead do

```python
try:
    import platform_specific_module
except ImportError:
    platform_specific_module = None
```

You can see there that I am catching the specific `ImportError` exception (not any exception!), which is what could happen when I execute the `import` statement.

For the same reason, you should never catch `Exception` or `BaseException`, or any exception raised by the Pacman infrastructure itself (as the ones used for tracking timeouts). This would amount to tampering with the Pacman infrastructure, which is pretty bad (check question above on that).

Most solutions won't require catching any exception, but if you happen to do/need so, you must catch specific exceptions and not the ones of the Pacman infrastructure.

## Should we remove this line `util.raiseNotDefined()` before starting our code or not? What does it do?

Yes, you should remove it - to figure out what it does I encourage you to look up its definition in `util.py` ;-)

## My editor shows an error trying to import pacman module
At line 32 of autograder.py (or perhaps elsewhere in different projects), you might see an underline with a warning message saying 'Import "pacman" could not be resolved'. This is not a problem, as the code is wrapped in a try/except block, so you can ignore this warning from your editor.

![Pacman import warning](img/pacman-import-warning.png)

## The autograder says `FAIL: Exception raised ...` but I am not sure which test case failed
Due to the structure of the autograder, it cannot tell which test threw the exception. Tests are run in alphabetical order, so you can check yourself. The test failing will be the one immediately after the last one that passed. E.g. `0-small-tree` in the screenshot below.

![Exception raised by test 0-small-tree](img/exception_test.png)
-----------------
# Project 0

## Do we have to handle edge cases? For example, for the `shopSmart` function, what should we do if a fruit is _not_ present in one of the shops?

For this project only (Project 0), since it is just designed to get you warmed up with python and git, you do not need to consider edge cases which are not mentioned in the project spec.

Specifically:

* for Q2, you should handle the case where the price list does not contain a fruit in the order, and return `None` as specified.
* for Q3, you do not need to handle the case where the shop does not contain one of the fruits in the order - you can assume _all_ shops will have all relevant fruit.

Having said that, for your own benefit, this is a great question to be thinking of, and you should feel free to handle the edge case if you would like. This is a great bonus activity that introduces you to some of the subtleties inherent in working with existing code-bases.

Note that, for all future projects you should consider edge cases carefully and handle them appropriately, even if we do not say so explicitly in the project spec. This is a critical skill for programming and will really test your detailed knowledge of the underlying algorithms that you will see in this course.

**Note:** in principle, a shop that misses one item in the order would just need to be ignored and not considered. However, this would mean that code in `shop.py` would have to be altered (which goes against what UC's specification!), because the predefined shop class contains its own function `getPriceOfOrder`, which does _not_ handle missing fruit in the way that Q2 requires.

One could import the function from Q2 and use that instead, but the function signatures then won't match, so one needs to create a wrapper in Q2 anyway, and it all gets a bit messy. Fundamentally if you use `getPriceOfOrder`, it will give wrong results for any shops which don't stock all your fruit, but that does seem to be the intended solution.

## Does the reference to 'pounds' in buyLotsOfFruit.py refer to weight (lb) or cost (£)?
The weight; this project was made in the US so uses US terminology, not UK.

-----------------
# Project 1

## Do we need to do all the "`*** YOUR CODE HERE ***`" method?

Not really. Just those parts that are relevant for the questions in the assessment.

Some parts are extension that may not be used in a particular edition of the course. For example, in the 2022 edition you don't have to complete `capsuleProblemHeuristic`.

## Can I import standard libraries?

Yes, as long as they are reasonable and do not contradict the spec. For example, importing `sys` to access `sys.maxsize` would be totally fine. Do not import libraries, though, that you wouldn't expect any Python install to include. Or do not use libraries or classes that go against the spec, for example by not using the data structures provided to you in `util.py`!

## What actions should I return in the search algorithms?

Check the actions in this class in `games.py`

```python
class Directions:
  NORTH = 'North'
  SOUTH = 'South'
  EAST = 'East'
  WEST = 'West'
  STOP = 'Stop'
```

## How can I represent a plan with no actions?

Either with an empty list or with a list with just action `Stop`.

## What counts as an expansion? I am getting too many expansions....

Basically, every time you call `problem.getSuccessors(.)`.

(It is not popping out from the queue, as we don't have access to that part of your code!)

So be careful not using that function for more than what is needed. When debugging, be careful, you may introduce [Heisenbug](https://en.wikipedia.org/wiki/Heisenbug)! :-)

One can implement the various search algorithms (e.g., DFS) doing one call to `getSuccessor()` per loop/node, as in the pseudo-code (e.g., book or slides).

## My solution works manually for `tinaMaze` but the authograder fails. The state format used in the autogarders tests are different from the Pacman game's in `tinaMaze`. What happens here?

Indeed, the test cases often have atomic states instead of `(x,y)` coordinates, but this should not affect your code at all. From the algorithms perspective, a state is (just) a "state", regardless of the representation. The autograder often checks corner cases which are not tested by the standard
mazes, which may be why you see it failing (despite your manual cases working).

## In Q7, can I take a heuristic from elsewhere (e.g., Google) and implement it?

The objective of the exercise is NOT to program in Python a solution that somebody else has invented/created. The fact is that we are not testing Python here or even coding skills per se alone. We are learning how to come up/create good heuristics ourselves, by thinking about the domain at hand and the way search works.

What we are interested in assessing for this question is your ability to understand what heuristics are and design them yourself. As a result, while searching online for heuristics **in general** would be fine (but we doubt useful here if you read the book), searching for a heuristic, even at a conceptual level, for this particular problem is definitively **not** OK.

Think about what some relaxations of the problem are, and how you might design a heuristic from those. There are a number of quite simple heuristics that do quite well, as well as some more sophisticated ones.

## In Q7, what timeout will be used? How do I know what timeout should I use?

The key point to understand here is *why do we use heuristics after all?* We use heuristics to guide the search---informed search---so that it runs _faster_.

OK, but _faster than what?_ Well, at least faster than if we do not use a heuristic, right? So, we can set the heuristic to just be `0` (by just doing `return 0` at the top of function `foodHeuristic`) and see how much it would take by running:

```shell
$ python pacman.py -l trickySearch -p AStarFoodSearchAgent -q

Path found with total cost of 60 in 1.5 seconds
Search nodes expanded: 16688
Pacman emerges victorious! Score: 570
Average Score: 570.0
Scores:        570.0
Win Rate:      1/1 (1.00)
Record:        Win
```

So it takes 1.9 seconds (in the cluster machines) when running the agent with an "empty" heuristic. What happens when we plugged our heuristic?


```shell
$ python pacman.py -l trickySearch -p AStarFoodSearchAgent -q

Path found with total cost of 60 in 0.3 seconds
Search nodes expanded: 255
Pacman emerges victorious! Score: 570
Average Score: 570.0
Scores:        570.0
Win Rate:      1/1 (1.00)
Record:        Win
```

As one can see the time was cut down to just 0.2 seconds (20% of the time when no heuristic is used!) and the number of nodes expanded to just 255. Note this is a very powerful heuristic (it expanded only 255 nodes!), and we are not expecting this to get full marks. There are still very fast implementations taking 0.5secs and expanding ~1500 nodes, way below the 7000 mark!

So, the question is not just whether the heuristic reduces the number of expansions, but also, ultimately, the search time.

When solving this question consider:

1. How good is your A* implementation?
2. How good is your heuristic?

Basically you are after a good enough A* implementation and a heuristic that _significantly improves_ A* when used without heuristic.

Remember that a heuristic is useful, only if gives benefit over not using it; otherwise what is the point of it? If your heuristic expands very few nodes, BUT it takes a lot of time to compute, then the heuristic will not be beneficial after all. Consider, what would be the very best heuristic you can use (but not useful)? ;-)

> [!NOTE]
The performance runs were done in the cluster machines. Your laptop may be faster. In my laptop, the above runs take 1 and 0.2 seconds, resp. To have an estimation how that compares with your machine, check [this question](https://github.com/RMIT-COSC1127-1125-AI24/AI24-DOC/blob/main/FAQ-PROJECTS.md#how-do-i-compare-the-speed-of-my-desktoplaptop-with-that-from-the-cluster-being-used-for-marking).

Finally, take note of the comment in the source code:

```
If you want to *store* information to be reused in other calls to the
    heuristic, there is a dictionary called problem.heuristicInfo that you can
    use. For example, if you only want to count the walls once and store that
    value, try: problem.heuristicInfo['wallCount'] = problem.walls.count()
    Subsequent calls to this heuristic can access
    problem.heuristicInfo['wallCount']
```

This could be a deal breaker and could move your heuristic performance from 30secs to 1sec.

## Are we allowed to use `mazeDistance` (or a modified version) when calculating our heuristic?

Yes, you certainly can, which is why it says the following in the comments:


> This might be a useful helper function for your ApproximateSearchAgent.

Be careful though - it is easy to imagine that if you call a function to do something, it is 'free', but if you look at the code in that function, you will soon realise that this function may take a lot of time itself. :-)

## Can we create a new BFS for the part 5? My implementation doesn't fit with my new state representation!

This is a good question. The answer is _no_ - you cannot and should not need to create a new BFS.

Search algorithms should be entirely generic and only interact through the interface defined at the top of `search.py` by the generic `SearchProblem` class.

Remember the key tasks in designing a search-based solution:

![sas](img/p1-search_repr.png)

This issue is about the first task: _representation_.

## In the feedback autograder, what does `expanded_states` means?

Basically, the number of times you have done expansion of nodes, that is, number of calls to `getSuccessors()`` method. Makes sense? :-)

## For Q9 cycle checking, should we check only a few levels, or all the way up to the root node?

While the book discusses both options, for project 1 you should implement a cycle check that goes all the way up to the initial state.

## In Q6 or Q7 I am getting `FAIL: inconsistent heuristic path` for a test case, what does this mean?

You have an inconsistent heuristic; i.e. it either 
- overestimates the true cost, or 
- it overestimates the difference between two nodes. (i.e. X and Y are neighbours, heuristic cost of X is 10, Y is 13, and the cost from X to Y is 2).

You will need to try to figure out why your heuristic is inconsistent, and fix it, or use an entirely different heuristic.

-----------------
# Project 2

## Inconsistent depth in minimax project 2, Q2 and careful use of `__init__`

So it looks like this issue is due to issues in calling constructors of parent classes (i.e. `__init__`). This can be a bit tricky, so here is the takeaway that is needed for this project:

If you want to add an `__init__` method into any (or all) of `MinimaxAgent`, `AlphaBetaAgent`, or `ExpectimaxAgent`, it should look like this:

```python
class MinimaxAgent(MultiAgentSearchAgent):
    def __init__(self, **kwargs):
    "*** YOUR CODE HERE ***"
    super().__init__(**kwargs)
```

This ensures that you aren't interfering with the arguments being passed through to the `MultiAgentSearchAgent` subclass. For anyone who wants to know why you need to do this and what that means, keep reading.

Let's imagine you want to add something to the constructor (i.e. the `__init__` method) of `MinimaxAgent`, for whatever reason. Your first attempt might look like:

```python
class MinimaxAgent(MultiAgentSearchAgent):
    def __init__(self):
    self.foo = 0 # initialise foo
```

This should fail with the following `error: TypeError: __init__()` got an unexpected keyword argument 'depth'.

Why is that? Well, the test harness is trying to call `__init__()` on `MultiAgentSearchAgent` to pass in the depth (and potentially `evalFn`) argument. Your new constructor now overwrites the original constructor of `MultiAgentSearchAgent`, and it isn't expecting any arguments, hence the error. What you want to do is call the parent constructor from within your constructor, to make sure that you aren't interfering with the original code. You can try to do so with the `super()` keyword like so:

```python
class MinimaxAgent(MultiAgentSearchAgent):
    def __init__(self):
    self.foo = 0 # initialise foo
    super().__init__()
```

But this still gives the same error, as you haven't passed through the arguments. You can pass them through manually like so:

```python
class MinimaxAgent(MultiAgentSearchAgent):
    def __init__(self, evalFn = 'scoreEvaluationFunction', depth = '2'):
    self.foo = 0 # initialise foo
    super().__init__(evalFn, depth)
```

However this runs into a number of problems:

If you have multiple parent classes (either directly or indirectly), you don't know which arguments to pass.
It duplicates code (including default arguments), now a change to one class needs to be made in many places.
It requires you to know exactly what the parent class is doing, which is not ideal.

This is where `**kwargs` comes in. For our purposes we can think of `**kwargs` as a dictionary that store an unlimited number of keyword arguments to a function, where we don't have to know what they are. This allows you to pass then on to other functions from parent classes, but you can also access them like any other dictionary:

```python
class MinimaxAgent(MultiAgentSearchAgent):
    def __init__(self, **kwargs):
    self.foo = 0 # initialise foo
    print("Minimax depth: ", kwargs['depth'])
    super().__init__(**kwargs)
```

More details about super can be found [here](https://stackoverflow.com/questions/2399307/how-to-invoke-the-super-constructor-in-python) (although it lacks discussion of arguments), and details about kwargs [here](https://stackoverflow.com/questions/3394835/use-of-args-and-kwargs).

## Can we apply a "magic number" such as -9999 in our evaluation functions, as part of our logic not simply an arbitrary "return -9999"?

You would not be marked down for using a number like that - however if you really want a very large number, you might consider using `math.inf` instead, or even `float('inf')`.

## In Q4, what does it mean an adversary which chooses amongst their `getLegalActions` uniformly at random?

All it means is that the other players in the game are acting randomly, with no bias towards any action: all legal actions have the same chance of being executed. For example, if player 2 has three legal moves: left, down and up, then it will choose left with 33% chances, down with 33% chances and up with 33% chances.

## The results of the feedback autograder with graphics and without graphics are very different! My system works without graphics but times out with graphics and I lose all games, why?

When you run it with graphics, it's just running out of time because it takes a while for the games to display. No need to worry, we will be grading _without_ graphics so it will not timeout for that reason (if you just run `python autograder.py` without specifying a question, it runs without graphics as default). The graphics are just there so you can see the behaviour of your agents more clearly.

## When I run the autograder I get the message _"has not SIGALRM"_, why?

That message is fine, you can ignore it. It is mostly a debug message and we will probably remove it for future projects. Thanks!

## What is a reasonable time for Question 5?

It is hard to give precise times, as that will depend on what hardware you are running on. See [question above](#how-do-i-compare-the-speed-of-my-desktoplaptop-with-that-from-the-cluster-being-used-for-marking) regarding how to compare the relative speed of your machine with that of the cluster machines used for marking.

On our own desktop, our solution runs the entire `Q5` from start to finish  in ~5 seconds (`python autograder.py -q q5 --no-graphics`). For reference, if we just `return 0`, it takes ~3 seconds just to run the games themselves.

Now here is how it runs our solution in the cluster:

```shell
$ python autograder.py -q q5 --no-graphics

Question q5
===========
Playing 10 games with seed 0 and timeouts set to 120 seconds.
Pacman emerges victorious! Score: 1359
Pacman emerges victorious! Score: 1161
Pacman emerges victorious! Score: 1338
Pacman emerges victorious! Score: 1283
Pacman emerges victorious! Score: 1340
Pacman emerges victorious! Score: 1346
Pacman emerges victorious! Score: 1151
Pacman emerges victorious! Score: 1277
Pacman emerges victorious! Score: 1311
Pacman emerges victorious! Score: 1191
Average Score: 1275.7
Scores:        1359.0, 1161.0, 1338.0, 1283.0, 1340.0, 1346.0, 1151.0, 1277.0, 1311.0, 1191.0
Win Rate:      10/10 (1.00)
Record:        Win, Win, Win, Win, Win, Win, Win, Win, Win, Win
*** PASS: p2-multiagent-grader/marking-packs/02.AI22/q5/grade-agent.test (6 of 6 points)
***     1275.7 average score (2 of 2 points)
***         Grading scheme:
***          < 500:  0 points
***         >= 500:  1 points
***         >= 1000:  2 points
***     10 games not timed out (1 of 1 points)
***         Grading scheme:
***          < 0:  fail
***         >= 0:  0 points
***         >= 10:  1 points
***     10 wins (3 of 3 points)
***         Grading scheme:
***          < 1:  fail
***         >= 1:  1 points
***         >= 5:  2 points
***         >= 10:  3 points
=====> Time taken for question:  5.831640720367432
```

As you can see, our solution less than 6 seconds in the cluster.

## Is there a way to run the evaluation function in Question 5 in harder setting or with more ghosts?

Try:

```shell
$ python .\pacman.py -p ExpectimaxAgent -a evalFn=better
```

or even harder!:

```shell
$ python .\pacman.py -p ExpectimaxAgent -a evalFn=better -l originalClassic
```

Alternatively: 
if you go into `test_cases/q5/grade-agent.test`, you can change the autograder to use different maps by modifying the `layoutName` field. You can also add more ghosts by modifying the ghosts field to this value: `"[RandomGhost(1), RandomGhost(2)]"`.

But we only care about the agents performance in the setting run by the autograder under original settings. 

## Unlike in P1, we are not given explicit pseudocode, can we still follow the book?
Yes of course! The reason we don't stress this point in this assignment is that there is really only one way to do Minimax, so there is not such an issue with little subtle differences.

## Can I reuse code from P1 in my heuristic evaluation function (e.g. copy my A* search over?)
Yes!

## Autograder is passing Q1, but the scores from the games are negative, is this ok?
Yes, each timestep you lose 1 score. If the game goes for a very long time, you can have a negative score even if you eat all the food.

-----------------
# Project 3

## I want to get a head start and learn prolog now! How can I do it?
Good on you for looking ahead, I have found these helpful in the past. 

- An Introduction to Prolog (Appendix A). In: [An Introduction to Language Processing with Perl and Prolog](https://link.springer.com/chapter/10.1007/3-540-34336-9_16). Cognitive Technologies. 2006. Springer, Berlin, Heidelberg.
- https://www.metalevel.at/prolog

But also for everyone else don't worry, we will be releasing additional resources closer to the assignment. Things will make more sense once you have seen predicate logic in class.

## GitHub is telling me all checks have failed, but some tests are passing on my machine, is this a problem?

Some of you have noticed that for this project, you might see something that looks like this in your feedback branch in your repo.

![Checks failed](img/GitHub-checks-failed.png)

While it says "All checks have failed" this is not a problem! All it means is that your latest code does not fully pass the provided unit tests. 

This is a feature of GitHub classrooms that was briefly mentioned in the spec: 

> This repo includes some unit testing cases to provide you with valuable feedback. The tests are run every time you push to your remote, but you can also run the tests locally via goal `run_tests/0` as follows: ...

The unit tests are run as a hook every time you push to GitHub, which allows us to track your progress in real time. This is just one more reason to make sure you are committing often, including code which is not fully complete!

The reason you are seeing all checks have failed, even when you have passed some the tests is that GitHub only knows about the top level. As far as GitHub is concerned, there is one test being run, that either passes or fails. But that is actually made of lots of test cases, grouped by exercise, which is where the 5 points are coming from. If you click on the details next to the failing check, you will see all the test output.

You may notice that all checks are failing on the feedback branch in particular, this is because that branch does not have any of your code in it, so it will always show as failing. This is not a problem.

## GitHub error on push `The following actions use a deprecated Node.js ...`
This is just a configuration issue behind the scenes for the GitHub automated testing (see above answer for more details). You can safely ignore.

## Is it ok to change the parameter structure of the predicates we are told to implement?
> eg:- `P(x)` could be changed to `P([H|T])`?

Yes, note this does not change the predicate signature itself, it is just changing the names used to refer to different parts of the argument.

## Is it ok to define multiple versions of the predicates (helpful for base and edge cases)?
Yes, and it would be almost impossible to complete the assignment without it.

## Is it ok to define helper functions?
Yes, these are called auxiliary predicates, and are in the spec already:
> You would probably need to use auxiliary predicates, and resort to recursive definitions.

## My solution prints false when the example doesn't, or warning: `Test tools_for_items_2: Test succeeded with choicepoint`
![Choice point example](img/prolog-choicepoint.png)

Both of these have the same root cause, and the short answer is that you don't need to worry about it. 

The longer answer is:
Fundamentally, the error is essentially saying that your predicate is finding only the one right answer, but in order to confirm that is the single correct answer it needs to backtrack through a bunch of choices it makes along the way, which is inefficient. However, a good solution will be written such that finding the single correct answer does not leave any unresolved choices, so it can return immediately.
From my perspective, it would be better if you could get rid of this, but in this course we will not penalise you for this behaviour. Usually we try to remove those dummy choice points, but sometimes it is not possible or it becomes a mess. 


## Best way to check empty list in Prolog
> Are there any differences/considerations/trade-offs between \= [] and \+ length(someList, 0) ?

The first reads easier and more direct, so I wold use that. 

In some circumstances you might even get different results. If someList is only partially instantiated; i.e. it is [2,3,X] where X is still a free variable that may be a continuation of the list, then length may be undefined, but at least 2. In this case the first is clear, [2,3,X] \= [], but I don't know whether prolog would be able to tell that length>=2 and therefore the second would also fail.

And if you want to check if it is a list or not, just use is_list/1

## Do we need to handle cyclic dependencies?

> e.g. where an item has itself as an ingredient, or a tool required to make an item, has that item as an ingredient.

No, for this assignment, it is safe to assume that every recipe is possible to make even starting with nothing. That means, no cycles in ingredients (because then it would be impossible to craft the item), and also no cycles in tools (as it would make it impossible to craft the tools). 

## What do the question marks mean in the predicate: `tool_for_item(?Item, ?Tool)`?

These are the [argument mode indicators](https://www.swi-prolog.org/pldoc/man?section=argmode), `?` means it can be provided or not.

## I can't see the full output in prolog, I am getting dots instead indicating it continues. How can I see everything?

Press `w` after it prints the dots to see the full output.


-----------------
# Project 4

## What are 'Noise' and 'LivingReward' in Q3?
Living reward is the reward given to the agent at each time step regardless of the state it is in (for 'living' another timestep). 

Noise is the probability that the agent accidentally moves left/right instead of in the direction it meant to go.

## How should we come up with values for Q3? Do we just guess? Do we have to explain it?
You should definitely not be blindly guessing, but you may need to try a few informed guesses before you get the right answer. You do not need to explain your values.

Longer answer: There is no way to take the expected policy and somehow solve backwards to recover these parameter values, because the values are not unique. There are many (often infinitely many!) different parameter combinations that will lead to the same policy. 
Instead, you should use your understanding of Q-learning to understand which values will result in each of the indicated outcomes. Whether this can be done purely intuitively, or requires actual policy calculations, will depend on how deep your understanding is.

If it seems like a big ask to do this intuitively the only tip I have is that generally in these situations you want to consider extreme values for parameters because that will have the biggest effects.


## What do I need to do for Q7? The autograder passes without any new code.
If you have done all of the previous questions properly, it is very possible for Q7 to run correctly without any new code. It is essentially just applying your existing code to pacman (which is why it is only worth 1 mark). The intention is just for you to understand how the training process works, and to motivate Q8 with the failures of your Q-learning agent to win on the medium grid.

## The textbook algorithm for Value Iteration takes $\epsilon$ as a parameter, where is this in the project code?
The project uses a slightly different version of the algorithm, so there is no epsilon paramter. There is however, a variable that serves a similar purpose. As a hint, what is the point of epsilon in the original algorithm? How is that objective achieved in the project code?

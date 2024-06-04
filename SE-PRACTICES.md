# SE and GIT Best Practices

Besides the correctness and performance of your solutions, you _**must**_ **follow good and professional SE practices** in your projects, including good use of git version control and professional communication and team-work during your development.

Overall, you want to generate a meaningful git history that provides quality evidence of your working towards your solution.

These include:

* _Configure your git authorship_: set your name and email address correctly so that your commits have correct authorship information. Please access the commit history in your remote repo, and check your commits are linked to your GH username: your username in each commit should be "clickable"; if you cannot click on the user of a commit, then that user is wrong configured and you must fix it.
  * Read about this issue and how to correct it if wrong [here](https://docs.github.com/en/pull-requests/committing-changes-to-your-project/troubleshooting-commits/why-are-my-commits-linked-to-the-wrong-user).
* _Commit early, commit often (but meaningfully!):_ single or few commits with all the solution or big chunks of it is not good practice.
* _Use atomic logically-separate commits:_ avoid commits about many things or dummy commits; each commit should be about one interesting thing. You want to create a meaningful git history, that allows you to easily revert a past change. For that, you also don't want to flood your git history with tons of padding commits.
* _Use meaningful commit messages:_ as comments in your code, a commit message should clearly and succinctly summarize what the commit is about. Messages like "fix", "work", "commit", "changes" are poor and do not help us understand what was done. Check the nice posts [“Good Commit” vs “Your Commit”: How to Write a Perfect Git Commit Message](https://www.linkedin.com/pulse/good-commit-vs-your-how-write-perfect-git-victor-timi/) and [Git Best Practices – How to Write Meaningful Commits, Effective Pull Requests, and Code Reviews](https://www.freecodecamp.org/news/git-best-practices-commits-and-code-reviews/).
* _Never upload files:_ git should not be used as a storage service. Setup your system to do proper meaningful commits and do not use GitHub's upload button ever.
* _Never ever force push to repo:_ forcing will re-write your repo history and cause serious problems and interferences with our mirroring system. Instead use `git revert` to undo a commit by creating another commit. Check the FAQ for projects for more info on `git revert` (or search for it and learn how to use it).

Besides proper commit behavior to obtain a clean and meaning history, you should:

* _Use the Issue Tracker:_ use issues to keep track of tasks, enhancements, and bugs for your projects. They are also a great way to collaborate in a team, by assigning issues and discussing on them directly. Check GitHub [Mastering Issues Guide](https://guides.github.com/features/issues/).
* _Follow good workflow and use branches:_ use the standard branch-based development workflow; it will make your team much more productive and robust! Check GitHub [Workflow Guide](https://guides.github.com/introduction/flow/). When merging or re-basing, squash commits _only_ when it will yield a better quality set of commits in the main branch; in general you should avoid squashing (e.g., do not squash commits that are by themselves meaningful).

In addition, if working in groups for a team-based project:

* _Commit evenly across team members_ (for team project/assignment components). This means there should be meaningful commits from _all_ participating members. Note that [peer programming](https://en.wikipedia.org/wiki/Pair_programming), which we encourage, does _not_ mean one member always or mostly acts as the "driver" and commit; *all* members should take turns, be the "driver" and commit to the repo.
  * When peer-programming, make use of the [co-author facility](https://docs.github.com/en/github/committing-changes-to-your-project/creating-and-editing-commits/creating-a-commit-with-multiple-authors) in GitHub to be accounted in the contributions. See [this post](https://gitbetter.substack.com/p/how-to-add-multiple-authors-to-a) and [this post](https://github.blog/2018-01-29-commit-together-with-co-authors/) as well about co-authors commits. You can conveniently include multiple co-authors to a commit via GitHub Desktop or via VScode (or otherwise by writing special commit messages) as explained in the links given.
* _Communicate in the GitHub (Discussions, Issues, Pull Requests, and Projects):_ in team projects, members are expected to communicate and coordinate in an adequate, professional, and efficient manner. In GitHub, teams can use Discussions, Issues and Pull Requests, and Projects within the repo of the project. Video and voice chats outside of GitHub are permissible (and encouraged), but communication and coordination should not be limited to that.

Poor SE and version control practices can have a significant impact in the final mark of an assessment. For example, a single commit with all the solution will attract zero marks overall, even if the solution does perform perfectly.

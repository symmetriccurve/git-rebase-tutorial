# A Simple git-rebase tutorial

Image you are working a team building a project and each of you are given a different feature to build and commit the progress code to master branch(Consideraing not to disturb other team members code)

Now you go create a a-feature branch(Yes! the name of the branch is "a-feature") out of your master branch based(remember the word based here and we will get back to it later) on last commit on the master.

Lets assume the time you branched out  of the master, the master was on D-Commit(Image as referred below)

You work hard and create some awesome code lines and when you feel the code is stable you commit the code to a-feature branch saying a1-commit, 

you go along and do another commit on a-feature say a2-commit. 

Out of the blue you see the mater branch and see someone has committed the master branch(Say E-Commit), Oh Wait ! 

E-Commit is not part of my branch since my branch is knows only up to D-commit.

Panic mode enabled !
How to I get this code into the branch so I can keep up with master branch and also work on the feature branch. 

git-rebase is at your rescue. 

Remember that the E-Commit was the base of the a-feature branch now I have to rebase (Aha !!), let's re base to re configure the base of the a1-feature branch to have new base which is E-Commit.

>git rebase master

Voila !! You have all the changes from the master and you can continue to work on your feature. . . !! Oh WAIT !! I have another commit on master branch, 

Panic Mode disable ! Git rebase Enabled

![N|Solid](https://raw.githubusercontent.com/symmetriccurve/git-rebase-tutorial/a-feature/Git-Rebase-example.png)

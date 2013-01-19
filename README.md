Practice
========

Just fool around, try to get acquainted with GitHub and Git.

---

#### UPDATES:
* Please visit the [tutorial](http://www.datacomm.me/git.html).
* Please prove you're able to commit via the 'proof-of-commit' folder.

#### For team leads:
When you fork your own repository, *your* team's fork does not automagically update with
the `datacommies`' repo as pull requests get accepted and merged.
For example, `datacommies/Practice` has recently accepted and merged a pull request, and
suppose that there's a new file `homer-simpson.txt` from that pull request, you will not see this
on your own fork, `gigglyalbertwei/Practice`. Nor will you see any changes to any
existing files modified by this pull request.
I'll walk through step by step and explain how you can sync your repository with the
`datacommies` branch.

    ronb@riemann:~/Practice$ git remote #let's see what repositories I'm tracking
    datacomm-master #I made this previously
    origin  #my forked repo
    ronb@riemann:~/Practice$ git remote add hookay git@github.com # "hookay" is just to illustrate that you can name the remote repo anything you want
    ronb@riemann:~/Practice$ git remote
    datacomm-master
    hookay
    origin
    ronb@riemann:~/Practice$ git fetch hookay
    ronb@riemann:~/Practice$ git merge hookay

To summarize, the steps are:

    $ git remote #to see current remote repos
    $ git remote add <nameofremotebranch> <git_url>
    $ git fetch <nameofremotebranch>
    $ git merge <nameofremotebranch>

---

Alright guys.  Here's the deal.  If you haven't used Git or GitHub before, this will aid in your learning process.

First things first, read the [help pages](https://help.github.com/) (whichever relevent).

The basic workflow will (probably) be as follows:
* For the repo
* Make any neccessary changes, add files
* Make a pull request
* I will review the pull request, and merge the forks if approved

Good luck, have fun!

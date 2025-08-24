# Git
---

```terminal
# Update
>| git pull
>| git push -f
>| git log
 |
# Checkout
>| git checkout main
>| git checkout branchToRebase/dev
 |
# Rebase
>| git rebase origin/main branchToRebase/dev 
>| git rebase -i head~13
>| git rebase —continue
 |
# Merge
>| git merge --abort
 |
# Reset
>| git reset --hard origin/branchToRebase/dev
 |
# Manage reflog information
>| git reflog
 |
# Reset current HEAD to the specified state
>| git reset --hard a0d3fe6
 | List, create, or delete branches
>| git branch <release-branch-name> <commit-hash>
 |
# Cherry pick
>| git swith <la-branche>
>| git cherry-pick -x <commit-1>
```


### Resources

- https://comprendre-git.com/fr/commandes/
- https://www.freecodecamp.org/news/git-commands
- https://rachelcarmena.github.io/2018/12/12/how-to-teach-git.html
- https://nvie.com/posts/a-successful-git-branching-model/
- https://delicious-insights.com/fr/articles/bien-utiliser-git-merge-et-rebase/
- Visual Git Referance: http://marklodato.github.io/visual-git-guide/index-en.html
- https://www.freecodecamp.org/news/how-to-make-your-first-pull-request-on-github/
- https://medium.com/@porteneuve/getting-solid-at-git-rebase-vs-merge-4fa1a48c53aa

### Practice Git

- [Git reference docs](https://git-scm.com/docs/git)
-  https://learngitbranching.js.org/
- Git guide: https://guides.github.com/activities/hello-world/
- Introduction to Github: https://lab.github.com/
- http://git-school.github.io/visualizing-git/
- http://try.github.io/
- https://jdblischak.github.io/2014-09-18-chicago/novice/git/05-sshkeys.html#:~:text=Add%20your%20public%20key%20to%20GitHub&text=Login%20to%20github.com%20and,hit%20Add%20key%20to%20save


### Git Sheet
http://rogerdudler.github.io/git-guide/index.fr.html
https://www.git-tower.com/blog/git-cheat-sheet
https://devhints.io/
https://www.kevinkuszyk.com/tag/git-tips/


# Git

---

- `git rebase origin/main branchToRebase/dev` to start rebase
- git rebase -i head~13
- git re#flog
- git reset --hard a0d3fe6
- git branch <release-branch-name> <commit-hash>
- If you want to add specific commit to it use cherry pick : :fr: [https://delicious-insights.com/fr/articles-et-tutos/git-cherry-pick/](https://delicious-insights.com/fr/articles-et-tutos/git-cherry-pick/)

**command repo**

- npm run format && npm run lint
- rm -rf node_modules
- npm run dev
- npm run hub:install —force
- npm run lint:fix
- npm set strict-ssl false
- npm run test-storybook:docker
- npm run test-storybook:docker:update
- node -e 'console.log(process.env)'

## Merge Main branche to main

- Get last updates on main branch 🚨 _If you don’t do that you may lose commits_
  - `git checkout main` to go on main branch
  - `git pull` to get last commits
- Get last updates on your branchToRebase/dev 🚨 _If you don’t do that you may lose commits_
  - `git checkout branchToRebase/dev` to go on the branch
  - `git pull` to get last commits
  - If there are merge conflicts ⚠️
    - It’s possible if the history isn’t the same and commit ids are different for example
    - `git merge --abort` to stop the merge
    - `git reset --hard origin/branchToRebase/dev` to reset branch and get remote version
- Once the 2 branches are up-to-date, you can process the rebase
  - `git rebase origin/main branchToRebase/dev` to start rebase
  - if conflicts, go on VS and solve them
    - then `git rebase —continue` to continue rebase
  - `git log` to check the history
    - last commit of main is here
    - commits of your branch are here
  - try to build/run tests locally to be sure there are no rebase errors or something else
  - `git push -f` to push updates
    - It will “override” the branch ith new commit ids. If you have a task branch, maybe you’ll need to rebase _yourTaskBranch_ on _yourDevBranch_ with same process. Check commits are not duplicated

### GIT Resources

- Pour les nuls
- https://www.freecodecamp.org/news/git-commands
- https://rachelcarmena.github.io/2018/12/12/how-to-teach-git.html
- https://nvie.com/posts/a-successful-git-branching-model/
- https://delicious-insights.com/fr/articles/bien-utiliser-git-merge-et-rebase/
- Visual Git Referance: http://marklodato.github.io/visual-git-guide/index-en.html
- https://www.freecodecamp.org/news/how-to-make-your-first-pull-request-on-github/
- https://medium.com/@porteneuve/getting-solid-at-git-rebase-vs-merge-4fa1a48c53aa

### Practice Git

- https://learngitbranching.js.org/
- Git guide: https://guides.github.com/activities/hello-world/
- Introduction to Github: https://lab.github.com/
- http://git-school.github.io/visualizing-git/
- http://try.github.io/
- https://jdblischak.github.io/2014-09-18-chicago/novice/git/05-sshkeys.html#:~:text=Add%20your%20public%20key%20to%20GitHub&text=Login%20to%20github.com%20and,hit%20Add%20key%20to%20save.

### Mooc Git
https://openclassrooms.com/fr/courses/2342361-gerez-votre-code-avec-git-et-github

### Git Sheet
http://rogerdudler.github.io/git-guide/index.fr.html
https://www.git-tower.com/blog/git-cheat-sheet
https://devhints.io/
https://www.kevinkuszyk.com/tag/git-tips/


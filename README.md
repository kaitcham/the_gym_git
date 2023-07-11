# Bundle 1 Exercise 1

- git add .
- git commit -m "Add index.html"
- git push
- git checkout -b dev
- git checkout -b test
- git checkout dev
- git branch -D test

# Bundle 1 Exercise 2

- git stash -u
- git stash -u
- git stash -u
- git stash pop stash@{1}
- git stash pop stash@{1}
- git add .
- git commit -m "Unstash about page and home page"
- git push
- git stash pop || git stash pop stash@{0}

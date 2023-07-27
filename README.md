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

# Bundle 2 Exercise 1

```
Kait cham@DESKTOP-JBLRO4G MINGW64 /d/The Gym/the_gym_git (main)
$ git checkout -b ft/bundle-2
Switched to a new branch 'ft/bundle-2'

Kait cham@DESKTOP-JBLRO4G MINGW64 /d/The Gym/the_gym_git (ft/bundle-2)
$ git add services.html

Kait cham@DESKTOP-JBLRO4G MINGW64 /d/The Gym/the_gym_git (ft/bundle-2)
$ git commit -m"Add services page"
[ft/bundle-2 e24e176] Add services page
1 file changed, 11 insertions(+)
create mode 100644 services.html

Kait cham@DESKTOP-JBLRO4G MINGW64 /d/The Gym/the_gym_git (ft/bundle-2)
$ git push --set-upstream origin ft/bundle-2
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 2 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 452 bytes | 113.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote: https://github.com/kaitcham/the_gym_git/pull/new/ft/bundle-2
remote:
To https://github.com/kaitcham/the_gym_git.git

- [new branch] ft/bundle-2 -> ft/bundle-2
  Branch 'ft/bundle-2' set up to track remote branch 'ft/bundle-2' from 'origin'.

```

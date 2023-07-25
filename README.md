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

# Bundle 3 Exercise 1

```
The Gym@DESKTOP-CD5BQ3O MINGW64 ~/Desktop/Projects/the_gym_git (main)
$ git checkout -b ft/team-page
Switched to a new branch 'ft/team-page'

The Gym@DESKTOP-CD5BQ3O MINGW64 ~/Desktop/Projects/the_gym_git (ft/team-page)
$ git add .

The Gym@DESKTOP-CD5BQ3O MINGW64 ~/Desktop/Projects/the_gym_git (ft/team-page)
$ git commit -m"Add team.html"
[ft/team-page 6a37a02] Add team.html
 1 file changed, 11 insertions(+)
 create mode 100644 team.html

The Gym@DESKTOP-CD5BQ3O MINGW64 ~/Desktop/Projects/the_gym_git (ft/team-page)
$ git push
fatal: The current branch ft/team-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/team-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


The Gym@DESKTOP-CD5BQ3O MINGW64 ~/Desktop/Projects/the_gym_git (ft/team-page)
$ git push --set-upstream origin ft/team-page
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 8 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 679 bytes | 679.00 KiB/s, done.
Total 6 (delta 3), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (3/3), completed with 2 local objects.
remote:
remote: Create a pull request for 'ft/team-page' on GitHub by visiting:
remote:      https://github.com/kaitcham/the_gym_git/pull/new/ft/team-page
remote:
To https://github.com/kaitcham/the_gym_git.git
 * [new branch]      ft/team-page -> ft/team-page
branch 'ft/team-page' set up to track 'origin/ft/team-page'.

The Gym@DESKTOP-CD5BQ3O MINGW64 ~/Desktop/Projects/the_gym_git (ft/team-page)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

The Gym@DESKTOP-CD5BQ3O MINGW64 ~/Desktop/Projects/the_gym_git (main)
$ git checkout -b ft/contact-page
Switched to a new branch 'ft/contact-page'

The Gym@DESKTOP-CD5BQ3O MINGW64 ~/Desktop/Projects/the_gym_git (ft/contact-page)
$ git checkout ft/team-page
Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.

The Gym@DESKTOP-CD5BQ3O MINGW64 ~/Desktop/Projects/the_gym_git (ft/team-page)
$ git log
commit 6a37a0299f2b33de64d4a0df1caa17ec589f0db6 (HEAD -> ft/team-page, origin/ft
/team-page)
commit 6a37a0299f2b33de64d4a0df1caa17ec589f0db6 (HEAD -> ft/team-page, origin/ft
/team-page)
commit 6a37a0299f2b33de64d4a0df1caa17ec589f0db6 (HEAD -> ft/team-page, origin/ft
/team-page)
Author: kaitcham <chams4f@gmail.com>
Date:   Tue Jul 25 09:54:17 2023 +0200

    Add team.html
The Gym@DESKTOP-CD5BQ3O MINGW64 ~/Desktop/Projects/the_gym_git (ft/team-page)
$ git checkout ft/contact-page
Switched to branch 'ft/contact-page'

The Gym@DESKTOP-CD5BQ3O MINGW64 ~/Desktop/Projects/the_gym_git (ft/contact-page)
$ git cherry-pick 6a37a0299f2b33de64d4a0df1caa17ec589f0db6
[ft/contact-page 00f678f] Add team.html
 Date: Tue Jul 25 09:54:17 2023 +0200
 1 file changed, 11 insertions(+)
 create mode 100644 team.html

The Gym@DESKTOP-CD5BQ3O MINGW64 ~/Desktop/Projects/the_gym_git (ft/contact-page)
$ git add contact.html

The Gym@DESKTOP-CD5BQ3O MINGW64 ~/Desktop/Projects/the_gym_git (ft/contact-page)
$ git commit -m"Add contact.html"
[ft/contact-page 4f26b8b] Add contact.html
 1 file changed, 11 insertions(+)
 create mode 100644 contact.html

The Gym@DESKTOP-CD5BQ3O MINGW64 ~/Desktop/Projects/the_gym_git (ft/contact-page)
$ git push --set-upstream origin ft/contact-page
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 8 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 690 bytes | 690.00 KiB/s, done.
Total 6 (delta 3), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (3/3), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/contact-page' on GitHub by visiting:
remote:      https://github.com/kaitcham/the_gym_git/pull/new/ft/contact-page
remote:
To https://github.com/kaitcham/the_gym_git.git
 * [new branch]      ft/contact-page -> ft/contact-page
branch 'ft/contact-page' set up to track 'origin/ft/contact-page'.

The Gym@DESKTOP-CD5BQ3O MINGW64 ~/Desktop/Projects/the_gym_git (ft/contact-page)
$ git checkout -b ft/faq-page
Switched to a new branch 'ft/faq-page'

The Gym@DESKTOP-CD5BQ3O MINGW64 ~/Desktop/Projects/the_gym_git (ft/faq-page)
$ git add faq.html

The Gym@DESKTOP-CD5BQ3O MINGW64 ~/Desktop/Projects/the_gym_git (ft/faq-page)
$ git commit -m"Add faq.html"
[ft/faq-page 0a7606b] Add faq.html
 1 file changed, 11 insertions(+)
 create mode 100644 faq.html

The Gym@DESKTOP-CD5BQ3O MINGW64 ~/Desktop/Projects/the_gym_git (ft/faq-page)
$ git push
fatal: The current branch ft/faq-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/faq-page

Revert "Add team.html"

[ft/faq-page 5c70070] Revert "Add team.html"
 1 file changed, 11 deletions(-)
 delete mode 100644 team.html

```

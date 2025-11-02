# kickers: workflow automators

# ABOUT

kickers automate common development workflows, such as syncing git changes between local and remote repositories. Workflows are customizable on a per-repository basis.

# EXAMPLE

```console
$ kick
+ git fetch --all --tags
Fetching gh-mcandre
Fetching gh-mcandre-2
+ git add .
++ git status --porcelain
+ '[' -n 'M  .kickers/kick' ']'
+ git commit -m up
[main a81ea0a] up
 1 file changed, 2 insertions(+), 3 deletions(-)
+ git pull
Current branch main is up to date.
+ git push
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 10 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (4/4), 395 bytes | 395.00 KiB/s, done.
Total 4 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To github.com:mcandre/kick-test.git
   f11346c..a81ea0a  main -> main
+ git push --tags
Everything up-to-date
```

# REQUIREMENTS

* [direnv](https://direnv.net/)

## Recommended

* [git](https://git-scm.com/)
* [GNU bash](https://www.gnu.org/software/bash/) 4+

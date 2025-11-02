# kickers: SDLC workflow automators

# ABOUT

kickers automate common development workflows, such as syncing git changes between local and remote repositories. Workflows are customizable on a per-repository basis.

# EXAMPLE

```console
$ kick -n -d
+ git fetch --all
+ '[' 1 -eq 1 ']'
+ date
+ git add .
++ git status --porcelain
+ '[' -n 'M  .kick' ']'
+ git commit -m up
[main 8a6fbc8] up
 1 file changed, 1 insertion(+), 1 deletion(-)
+ git pull
Current branch main is up to date.
+ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 10 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 370 bytes | 370.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To github.com:mcandre/kickers.git
   d189e5c..8a6fbc8  main -> main
+ git fetch --tags
+ git push --tags
Everything up-to-date
```

# REQUIREMENTS

* [direnv](https://direnv.net/)

## Recommended

* [git](https://git-scm.com/)
* [GNU bash](https://www.gnu.org/software/bash/) 4+

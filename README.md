# kickers: SDLC workflow automators

# ABOUT

kickers automate common development workflows. Workflows are customizable on a per-repository basis.

# EXAMPLE

```console
$ kick
(syncs local & remote git changes)
```

See `kick -h` for more options.

# REQUIREMENTS

* [direnv](https://direnv.net/) 2

## Recommended

* [git](https://git-scm.com/) 2.46.1+
* [GNU bash](https://www.gnu.org/software/bash/) 4+

# SETUP

1. Install direnv.
2. Register per-user and/or per-project kicker scripts.

The example [.kickers/kick](.kickers/kick) script automates common git operations.

## REGISTER PER-USER KICKER SCRIPTS

```console
$ mkdir -p ~/.kickers
$ cp global.envrc ~/.envrc
$ direnv allow
$ cp kickers/.kickers/kick ~/.kickers
$ chmod +x ~/.kickers/kick
```

## REGISTER PER-PROJECT KICKER SCRIPTS

```console
$ cd <project>
$ mkdir -p .kickers
$ cp .../kickers/sample.envrc ~/.envrc
$ direnv allow
$ cp .../kickers/.kickers/kick .kickers
$ chmod +x .kickers/kick
```

👟

# gitgrep

Search the git repository in the current directory for a given string.


# Overview

This script searches the git repository in the current directory for a given string.


# Usage

## General Help

Call the script with the -help as argument to get the help function:

```bash
$ gitgrep --help
```


## Help about a command:

To get the help about a command, call the script with the command and the --help option:

```bash
$ gitgrep search --help
```

## Sample Search

```bash
$ gitgrep search "my search string" -a
```


## Sample Search using Diff

```bash
$ gitgrep search "my search string" -a -d
```


## Sample Search using Diff between two commits

```bash
$ gitgrep search "my search string" -d -h 10f6b91b4f624bf67e815d0df74bc5777c2696f2 -h 36937ed0f7703b96d0279d7ee1c78c83eb6315d0
```

The first hash is the more recent hash, the second hash is the older hash. The script will show the differences between the two commits.

## Raw output

```bash
$ gitgrep search "my search string" -a -r
```

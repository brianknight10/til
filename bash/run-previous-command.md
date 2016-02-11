# Run Previous Command

Previous run commands can be viewed with the `history` command.

```shell
$ history
10048 git checkout master
10049 gpr
10050 rake
```

You can pipe this list to `grep` to find something particular.

```shell
$ history | grep git
10048 git checkout master
```

With these lists, you can rerun any command using `!n`.

```shell
$ !10048
Already on 'master'
```

You can also use `CTRL-R` and then type in the first few letters of a command, and bash will reverse search for that command.

```shell
$ (reverse-i-search)`': git c
$ git checkout master
Already on 'master'
```
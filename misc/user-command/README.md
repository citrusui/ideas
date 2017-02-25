# `user` Command

Suppose you are reading an online tutorial which asks you to locate your user directory, typically found under `/home`, `/Users`, or `$HOME`.

Using the `$HOME` variable is always an option, but an individual may want more control over _which_ user directory is opened.

## Concepts

### First-run

```sh
$ cp recipe.md `user`/Documents

Multiple user directories exist. Choose one:
1: /home/Users/Charles
2: /home/Users/Nancy
3: /home/Users/Sam

# Individual provides input...

Save this preference? [y/N]: y
```

### Configuration

```sh
$ user --config default="/home/Users/Charles" # user will load this directory when run without parameters
$ user --config path="/home/Users:/shared/Users" # user accounts will be loaded from these directories
```

Todoist CLI client
===

[Todoist](https://todoist.com/) CLI Client, written in Golang.

## Description

[Todoist](https://todoist.com/) is a cool TODO list web application.
This program will let you use the Todoist in CLI.

## Demo (with [peco](https://github.com/peco/peco))

### Add Task

![Add task](https://cloud.githubusercontent.com/assets/6121271/19836528/6ed99956-9ee6-11e6-85b0-7539393d803b.gif)

### Close Task

![Close task](https://cloud.githubusercontent.com/assets/6121271/19836531/7c399218-9ee6-11e6-974c-9dd59ced13a5.gif)

## Usage

```
$ todoist --help
NAME:
   todoist - Todoist CLI Client

USAGE:
   todoist [global options] command [command options] [arguments...]
   
VERSION:
   0.2.1
   
COMMANDS:
     list, l    Shows all tasks
     add, a     Add task
     modify, m  Modify task
     close, c   Close task
     labels     Shows all labels
     projects   Shows all projects
     karma      Shows karma
     sync, s    Sync cache
     help, h    Shows a list of commands or help for one command

GLOBAL OPTIONS:
   --color        
   --help, -h     show help
   --version, -v  print the version
```

## Install

```
$ go get github.com/sachaos/todoist
```

### Register API token

When you run `todoist` first time, you will be asked your Todoist API token.
Please input Todoist API token and register it.

### Use with peco

**RECOMMENDED**

install *peco* and load `todoist_functions.sh` on your `.zshrc`, like below.

```
$ source "$GOPATH/src/github.com/sachaos/todoist/todoist_functions.sh"
```

#### keybind

```
<C-x> t t: select task with peco
<C-x> t p: select project with peco
<C-x> t l: select labels with peco
<C-x> t c: select task and close
```


## TODO

* DueDate set option
* Refactoring

## Author

[sachaos](https://github.com/sachaos)

# ![dvlp](media/logo.png)

> A command line tool for managing local projects.


## Install

```
$ curl https://raw.githubusercontent.com/kjbrum/dvlp/master/dvlp > ~/bin/dvlp
$ chmod +x ~/bin/dvlp
```


## Usage

```
dvlp - v0.0.1

A command line tool for managing local projects.

Usage:
    dvlp init
    dvlp config <project>
    dvlp start <project>

Tasks:
    cleanup          Remove all config files
    config           Set up the config file for a specific project
        <project>    Name of the project you want to run
    init             Initialize necessary config files
    list             List all projects with config files
    start            Run a project's tasks
        <project>    Name of the project you want to run
    update           Download the latest version
    version          Display the current version
```


## Config

#### DVLP_TASKS

The default tasks to run for a project. _(Be sure to separate each task with a comma)_

__Options:__

```
editor
    "path_to_folder"                 The path of a folder to open in an editor
terminal
    new [tab,window]                 Open a new tab/window
        "path_to_folder"
    split [top|right|bottom|left]    Split a pane
        "path_to_folder"
finder                               Open a folder in a new Finder window
    "path_to_folder"

"path_to_folder" default = $DVLP_PROJECT_DIR/<project>
```

__Default:__

editor,terminal,finder

#### DVLP_EDITOR

The default text editor application.

__Options:__

- sublime

__Default:__

sublime


#### DVLP_TERMINAL

The default terminal application.

__Options:__

- iterm

__Default:__

iterm

#### DVLP_PROJECT_DIR

The folder your local projects are in.

__Default:__

/www/sites/


## To-Do
- Get the base tasks working
    - editor
    - terminal
        - new [tab|window]
        - split [vertical|horizontal]
    - finder
- Add support for additional tasks
    - Build Tools
        - [grunt|gulp|npm] "task to run" _(run a build tool task)_
    - Tests?
- Add support for additional editors
    - atom
    - brackets
    - textmate
    - coda
- Add support for additional terminals
    - terminal
- Add Bash autocomplete
- Add more information to README
    - Default config file
    - Project config files
- Take a screencast of actually using it
- ~~Add a `config` command for easily creating a config file for a project~~
- ~~Add an `update` command for downloading the most recent version~~
- ~~Set up config file (default)~~
    - ~~Default tasks to run (editor,terminal,finder)~~
    - ~~Editor (Sublime Text)~~
    - ~~Terminal (iTerm)~~
    - ~~Base destination for project folder (/www/sites)~~
- ~~Config file for individual projects with a default fallback~~
    - ~~Default tasks, editor, and terminal~~


## License

Copyright © [Kyle Brumm](http://kylebrumm.com). Free to use on whatever and may be redistributed under the terms specified in the [license](LICENSE.md).

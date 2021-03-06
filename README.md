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
        <project>    Name of the project of which you want to remove config files
    config           Set up the config file for a specific project
        <project>    Name of the project you want to run
    init             Initialize necessary config files
    list             List all projects with config files
    start            Run a project's tasks
        <project>    Name of the project you want to run
    update           Download the latest version of dvlp
    version          Display the current version
```


## Config

#### DVLP_TASKS

The default tasks to run for a project. _(Be sure to separate each task with a comma)_

__Options:__

```
editor
    "path/to/folder"                 The path of a folder to open in an editor
terminal
    new [tab,window]                 Open a new tab/window
        "path/to/folder"
    split [top|right|bottom|left]    Split a pane
        "path/to/folder"
finder                               Open a folder in a new Finder window
    "path/to/folder"

"path/to/folder" default = $DVLP_PROJECT_DIR/<project>
```

__Default:__

editor,terminal,finder

#### DVLP_EDITOR

The default text editor application.

__Options:__

- sublime text

__Default:__

sublime text


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
- Call `dvlp_config` when setting up the default config (DRY)
- Get the base tasks working
    - editor
        - "path/to/folder"
    - terminal
        - new [tab|window]
            - "path/to/folder"
        - split [vertical|horizontal]
            - "path/to/folder"
    - finder
        - "path/to/folder"
- Add support for build tools (plugin?)
    - [grunt|gulp|npm] "task to run" _(run a build tool task)_
- Add support for time tracking (plugin?)
    - harvest
    - toggl
- Add support for additional editors (plugin?)
    - atom
    - visual-studio
    - brackets
    - textmate
    - coda
- Add support for additional terminals
    - terminal
    - iterm
- Add Bash autocomplete
- Add more information to README
    - Default config file
    - Project config files
- Add support for default settings
- Take a screencast of actually using it
- Make additional support work in the form of "plugins"
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

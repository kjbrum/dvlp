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
    dvlp start <project>

Tasks:
    cleanup          Remove all the config files
    init             Set up the project files
    list             List all available projects
    start            Set up a project
        <project>    Name of the project you want to work on
    update           Download the latest version of dvlp
    version          Display the current version
```


## Config

#### DEFAULT_TASKS

The default tasks to run for a project. _(Be sure to separate each task with a comma)_

__Options:__

- editor
- terminal
- finder

__Default:__

editor, terminal, finder

#### DEFAULT_EDITOR

The default text editor application.

__Options:__

- sublime
- atom
- brackets
- textmate
- coda

__Default:__

sublime


#### DEFAULT_TERMINAL

The default terminal application.

__Options:__

- iterm
- terminal

__Default:__

iterm

#### PROJECT_DIR

The folder your local projects are in.

__Default:__

/www/sites/


## To-Do

- Handle many different tasks
    - Terminal
        - new [tab,window] _(opens a new window/tab)_
        - split [top,right,bottom,left] _(splits a pane)_
    - Editor
        - editor "/www/sites/project/content/themes/theme-name" _(opens file/folder in an editor)_
    - Finder
        - open "/www/sites/project" _(opens file/folder in Finder)_
    - Build Tools
        - [grunt,gulp,npm] "task to run" _(run a build tool task)_
- Add more information to README
    - Default config file
    - Project config files
- Add Bash autocomplete
- Prompt the user to enter a new projects config values
- Add an `update` task for downloading the most recent version
- Take a screencast of actually using it
- ~~Set up config file (default)~~
    - ~~Default tasks to run (editor,terminal,finder)~~
    - ~~Editor (Sublime Text)~~
    - ~~Terminal (iTerm)~~
    - ~~Base destination for project folder (/www/sites)~~
- ~~Config file for individual projects with a default fallback~~
    - ~~Default tasks, editor, and terminal~~


## License

Copyright © [Kyle Brumm](http://kylebrumm.com). Free to use on whatever and may be redistributed under the terms specified in the [license](LICENSE.md).

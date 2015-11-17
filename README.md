# dvlp

> A command line tool for easily getting started on projects.


## Install

```
$ curl https://raw.githubusercontent.com/kjbrum/dvlp/master/dvlp > ~/bin/dvlp
$ chmod +x ~/bin/dvlp
```


## Usage

```
dvlp - v0.0.1

A command line tool for easily getting started on projects

Usage:
    dvlp <project>

Tasks:
    init             Initialize the project config
    version          Display the current version
    cleanup          Cleanup config files
    <project>        The name of the project you want to setup

Options:
    --no-bs          Skip running BrowserSync
    --no-terminal    Skip opening the terminal
    --no-finder      Skip opening Finder
    --no-editor      Skip opening the editor
```


## To-Do

- ~~Set up config file (default)~~
    - ~~Default tasks to run (editor,terminal,finder)~~
    - ~~Editor (Sublime Text)~~
    - ~~Terminal (iTerm)~~
    - ~~Base destination for project folder (/www/sites)~~
- Open 2 new terminal windows: project root and the theme _(2 project roots if it's a patternlab)_
- Open the root of the project in an editor
- Open a finder window at the root of the project
- Make is so you can have a config file for individual projects
    - Ability to run Grunt tasks _(BrowserSync)_


## License

Copyright © [Kyle Brumm](http://kylebrumm.com). Free to use on whatever and may be redistributed under the terms specified in the [license](LICENSE.md).

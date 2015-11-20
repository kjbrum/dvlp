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

A command line tool for easily getting started on projects

Usage:
    dvlp init
    dvlp start <project>

Tasks:
    version          Display the current version
    init             Set up the project files
    cleanup          Cleanup config files
    start            Set up a project
        <project>    Name of the project you want to work on
    list             List all available projects

Options:
    --no-editor      Skip opening the editor
    --no-terminal    Skip opening the terminal
    --no-finder      Skip opening Finder
```


## To-Do

- ~~Set up config file (default)~~
    - ~~Default tasks to run (editor,terminal,finder)~~
    - ~~Editor (Sublime Text)~~
    - ~~Terminal (iTerm)~~
    - ~~Base destination for project folder (/www/sites)~~
- Open 2 new terminal windows: project root and the theme _(2 project roots if it's a patternlab)_
    - Allow specific settings "new tab,split right 'content/themes/theme-name,split bottom" (https://iterm2.com/applescript.html)
- Open the root of the project in an editor
- Open a finder window at the root of the project
- Make is so you can have a config file for individual projects
    - Ability to run Grunt tasks _(BrowserSync)_
- Add a better description of what the tool does
- Take a screencast of actually using it
- Add an `update` task for downloading the most recent version


## License

Copyright © [Kyle Brumm](http://kylebrumm.com). Free to use on whatever and may be redistributed under the terms specified in the [license](LICENSE.md).

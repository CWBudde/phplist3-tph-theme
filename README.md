# TPH theme (based on Trevelin) 
A Trevelin and thus bootstrap-based theme for [phpList 3](https://github.com/phpList/phplist3/)

[![Build Status](https://travis-ci.org/phpList/phplist-ui-bootlist.svg?branch=master)](https://travis-ci.org/phpList/phplist-ui-bootlist)

Bootstrap class names and extra html needed, inserted by jQuery with the script:
`js/phpList3ToBootstrap.js`

## Issues

please use the GitHub issues found here: https://github.com/CWBudde/phplist3-tph-theme/issues

## Getting started
If you are not going to develop, you don't need the /less and the /bootstrap directories:
* https://github.com/CWBudde/phplist3-tph-theme/tree/master/bootstrap
* https://github.com/CWBudde/phplist3-tph-theme/tree/master/less

If you are going to develop you need to follow this instructions:

### Building the project 
Requires nodejs & npm. See https://nodejs.org for setup.

### Install Grunt globally
``` 
sudo npm install -g grunt-cli
```
### Grunt plugins
To minify js we use this grunt plugins:

https://github.com/gruntjs/grunt-contrib-concat

https://github.com/gruntjs/grunt-contrib-uglify


### Install project dependencies
``` 
cd THEME_DIR # Replace THEME_DIR by theme path.
sudo npm install
```
### Watch the project
``` 
grunt watch
```
### Minify CSS
``` 
grunt less
```
Each time a less file is changed, style.css will be generated automatically.

### Minify the javascript
``` 
grunt concat
```
To unify all .js in one file: phplist_ui_bootlist.js

And then, to minify that file, you have to run:
``` 
grunt uglify
```

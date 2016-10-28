# grunt-doxdox

> Generate documentation with doxdox.

[![NPM Version](http://img.shields.io/npm/v/grunt-doxdox.svg)](https://www.npmjs.org/package/grunt-doxdox)

## Installation

```bash
$ npm install grunt grunt-doxdox --save-dev
```

## Usage

### Basic Options

```javascript
module.exports = function (grunt) {

    grunt.loadNpmTasks('grunt-doxdox');

    grunt.initConfig({
        'doxdox': {
            'dev': {
                'inputs': ['facade.js'],
                'output': 'docs.html'
            }
        }
    });

    grunt.registerTask('default', ['doxdox']);

}
```

### Custom Configuration Options

```javascript
module.exports = function (grunt) {

    grunt.loadNpmTasks('grunt-doxdox');

    grunt.initConfig({
        'doxdox': {
            'dev': {
                'inputs': ['script.js'],
                'output': 'docs/index.html',
                'config': {
                    'title': 'Sample Title',
                    'description': 'Lorem ipsum dolor sit amet, consectetur adipisicing elit',
                    'layout': 'docs/template.hbs'
                }
            }
        }
    });

    grunt.registerTask('default', ['doxdox']);

}
```

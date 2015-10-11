# es6-boilerplate
Boilerplate for authoring in ES6 and publishing in ES5.

## Scripts
```sh
$ npm run
Lifecycle scripts included in es6-boilerplate:
  test
    mocha --compilers js:espower-babel/guess test/*.js

available via `npm run-script`:
  build
    babel src --out-dir lib
  watch
    babel src --out-dir lib --watch
  test-watch
    mocha --watch --compilers js:espower-babel/guess test/*.js
  lint
    eslint src test
```

## How to use
```sh
# start new project from boilerplate
$ git clone --depth 1 git@github.com:tsuchikazu/es6-boilerplate.git new-project
$ cd new-project/
$ rm -rf .git
$ git init
$ git add .
$ git commit -m 'Initial Commit'
$ hub create -d 'Description for new-project'
$ git push

# edit for new project
$ sed -i -e "s/es6-boilerplate/new-project/g" README.md package.json
$ vim package.json
...
```

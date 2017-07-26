# How to install baseline

1. Create your project directory.
2. ```cd``` into the directory and ```vi package.json``` 
3. ```vi package.json``` and copy the following config.
```
{
  "name": "static-cms-baseline",
  "version": "1.0.0",
  "description": "",
  "author": "Koji Miyauchi",
  "license": "MIT",
  "scripts": {
    "init": "./node_modules/.bin/webdev-baseline-init",
    "update": "./node_modules/.bin/webdev-baseline-update"
  },
  "dependencies": {
    "static-cms-baseline": "git+ssh://git@bitbucket.oicr.on.ca/~kmiyauchi/webdev_static-cms-baseline.git"
  }
}
```
4. ```npm install```
5. ```npm run init```

# Enable UMS

1. Make ```pages/ums.md``` published.
2. Comment in the ums entry in ```_app/configs/entries.js```
3. Include ```dist/footer_scripts.inc``` in ```_layout/default.tpl```

# Compile javascript App

1. ```cd _app```
2. ```npm install```
3. ```npm start``` or ```npm build``` to compile files.
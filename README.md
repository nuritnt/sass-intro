# sass-intro

This is a simple setup template for sass installation with npm to get you going.

## Installation


#### Install Node.js & NPM
```bash
$ sudo apt update

$ sudo apt install nodejs npm
```

#### Make sure you have the following folder structure
```
sass-intro  
├── build  
│    └── css  
│        └── (the CSS file will be compiled and created here - never write in this file!)  
└── src  
│    └── scss  
│         └── style.scss (write your scss styles here!)  
├── index.html  
├── package.json  
```


#### Initialise NPM and install SASS to your devDependencies
```bash
$ npm init
$ npm i sass --save-dev
```

#### Add this to your package.json
```json
"scripts": {
  "sass:watch": "sass --watch $(pwd)/src/scss:$(pwd)/build/css"
},
```

#### Run your NPM command
```bash
$ npm run sass:watch
```

#### Create a .gitignore and add your node_modules and compiled css files there
```.gitignore
# Untrack node_modules folders
node_modules/

# Untrack compiled css files
build/
```

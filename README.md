# modern_responsive_portfolio
Directory structure: modern _portfolio > dist >index.html
                                                                      > scss > main.scss                                                                   
Node-sass is a library that provides binding for Node.js to LibSass, the C version of the popular stylesheet preprocessor, Sass. It allows you to natively compile .scss files to css at incredible speed and automatically via a connect middleware.Nov 15, 2018
node-sass - npm
https://www.npmjs.com/package/node-sass
go to view > terminal (to open a terminial)  or keyboard command: control `
npm init    (to create package.json file
Here is the detail of package.json file:
{
  "name": "modern_portfolio",
  "version": "1.0.0",
  "description": "Responsibe portfolio website",
  "main": "index.js",
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1"
},
chaged the above line to "scripts": { "sass": "echo \"Hello from sass script\"node-sass -w scss/ -o dist/css/ --recursive"  // this will compile all of our sass into regular css and put it in this file and we don't have to create css file.
  },
  "author": "Joanna Yang",
  "license": "MIT"
}
Run the following command to update the new major version of npm available 5.6.0 -> 6.5.0
npm i -g npm to update

Install the node-sass
npm i node-sass 
after install node-sass with success, now we can type: npm run sass
npm run sass

create the main.scss file and create a variable name: primary-color and assign it to #444
To create avariable in the main.scss file, we use the $primary-color. When the main.scss file save, the node-sass will automatically compile the main.scss file then create the css folder amd the main.css file in the dist directory and assign the background color in the main.css file.
Create the .gitignore file to include those file that we don't want that to be added to our repository. Save and close the gitignore file.
git init - initalize our repository by type git init to create a hidden folder call .git and all of our repositories where stuff goes in there 
git add .  - to add everything that we are done so far 
git commit -m "inital workflow setup"  - make a commit with a message "initlal workflow setup" to the respository right now it's jjust in the staging area.

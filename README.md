# Demo---Node.js-using-npm-for-dependency

- Step 1 //Go to project folder
- Step 2 init npm //to initialize the project/app with npm it will ask for certain details as follows
    2.1 name: <app_name>.app //make sure its in lowercase
    2.2 version //automatically shows just hit enter
    2.3 description //provide description of the project
    2.4 entry point: (index.js) <starting page>.js //by default it is index.js
    2.5 test command: //for test command
    2.6 git repository: //paste your git repository url if want to upload on git
    2.7 keywords: //keywords for the project
    2.8 license:// default is ISC
// After that it will show a preview of package.json which will store the above information as well as the the package that we inform using following command...

- Step 3 npm install <packagename> --save //this will import the lastest node recognized version of mentioned package for production
    Example npm install express --save 


- Step 4 npm install <packagename> --save //this will import the lastest node recognized version of mentioned package for development
    Example npm install express --save-dev

- Step 5
//if we push code to git or we share code/project to someone else we usally dont share with all packages i.e node_modules we just keep the package.json which have the record about all package in dependencies so after sharing or opening project if want to re-import/ re- install the node modules then we use command:
npm install //this command will install all the modules specified in package.json file in form of dependencies/ devdependencies 

- Step 6
//if we push code to git or we share code/project to someone else we usally dont share with all packages i.e node_modules we just keep the package.json which have the record about all package in dependencies so after sharing or opening project if want to re-import/ re- install the node modules then we use command:
npm install --production //this command will install all the modules specified in package.json file in form of dependencies i.e modules imported for production only


- Step 7
npm start // it is use to start the app/project
//in package under the script node we can specify which file to run when we use the 'npm start' commnand as follows:

..............
"scripts": {
    "start": "node app.js", // add this line of you want to use npm start command to start app else it will give an error
    "test": "echo \"Error: no test specified\" && exit 1"
  },
........

Conclusion: so there are 2 ways to start app using node <filename>.js 
or 
by npm start

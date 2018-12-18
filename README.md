# Bash-Script-To-Check-In-Git
It is git bash script to check in code for node js developer.

after completion of copy paste file content go to package json and add below line.

"{nameofnpmruncommand}":"sudo bash {pathoffile}/git_check_in.sh"

Example:-
{
...
 "scripts": {
    "test": "./node_modules/.bin/mocha",
    "start": "node server.js",
    "check_in": "git add . && git commit -m \"check in test\" && git push origin master",
    "Git_check_in":"sudo bash ./script/git_check_in.sh"
  },
  ....
  }
  
  
  Run Command:-
  npm run {nameofnpmruncommand}
  
  example:-
  npm run Git_check_in
  

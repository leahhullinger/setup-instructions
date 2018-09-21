# setup-instructions

### First GitHub

1. Create new repository on Github
2. Copy the repository url (clone/download button)

### Set up Your App/Folder Structure

1. Using terminal, create a new directory(folder)
    `mkdir new-folder-name`
  
2. cd into the new directory
    `cd new-folder-name`
    
3. `git init`
    `git remote add <git-repository-url>` (the repository url copied from github)

4. `create-react-app client`
5. `cd client`
6. `npm install axios`

7. ` cd .. ` (you should be in new-folder-name directory)
8. `mkdir server`
9. `cd server`
10. `npm init -y`
11. `npm install express body-parser cors`
12. `touch .gitignore`
13. `touch index.js`
14. `touch controller.js`

### Add Some Syntax

1. Open new-folder-name in vsCode
2. Add `node_modules` to the .gitignore file in the server folder
3. Go to index.js in the server folder and add the following code:

```
const express = require('express')
const bodyParser = require('body-parser')
const cors = require('cors')

const app = express();

app.use(bodyParser.json());
app.use(cors());

// endpoints will go here




app.listen(3005, () => {
console.log('listening on port 3005')
    
```

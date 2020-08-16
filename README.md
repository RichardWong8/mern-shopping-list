# 01: EXPRESS API & MONGODB
## Create a new project
```
npm init
```

## Install dependences
```
npm i express body-parser mongoose concurrently

body-parser: handle data that comes in
mongoose: interact with library
concurrently: run server client same time
```
```
npm i -D nodemon

-D: dev dependency
nodemon: automatically update server on save
```
## Modify package.json
```
modify scripts
"start": "node server.js"
"server": "nodemon server.js"
```

## Run server
```
npm run server
```

# 02: CLIENT SETUP & REACTSTRAP
## Create a react app
```
mkdir client
cd client
npx create-react-app .
```

## Modify client package.json
```
add
"proxy": "http://localhost:5000",
```

# Modify main package.json
```
add
"client": "npm start --prefix client",
"dev": "concurrently \"npm run server\" \"npm run client\""
```

# Install front end dependencies
```
npm i bootstrap reactstrap uuid react-transition-group

reactstrap: use bootstrap as React Components
```
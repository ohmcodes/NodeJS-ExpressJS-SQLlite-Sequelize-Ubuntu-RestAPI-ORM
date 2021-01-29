# NodeJS-ExpressJS-SQLlite-Sequelize-Ubuntu-RestAPI-ORM
NodeJS-ExpressJS-SQLlite-Sequelize-Ubuntu-RestAPI-ORM

This Repo will teach you how to Create RESTAPI using NodeJS ExpressJS Sequelize SQLite and Ubunt20, it has CRUD function as well and ORM for queries.

Here's the orignal video (must watch if you are iOS user):
https://www.youtube.com/watch?v=VDgXAw7VynQ&feature=emb_logo&ab_channel=DavidTang

## Requirements
- NodeJS
- ExpressJS
- SQLite3
- Sequelize
- Ubuntu20
- Nodemon
- Unzip
- body-parser
- Postman

## Resources
- [Sequilize docs](https://sequelize.org/master/index.html)
- [Sqlite3 Sample Database](https://www.sqlitetutorial.net/sqlite-sample-database/)
- [Postman](https://www.postman.com/downloads/)


## Install
```
npm i express sequelize sqlite3 body-parser --save
npm install --save-dev nodemon
```

## Start nodemon
```
npx nodemon app.js
```

## Setup SQLite3
```
sudo apt-get install sqlite3 libsqlite3-dev

Create db
sqlite3 ness.db

To SAVE
.save ness.db

To QUIT
.quit
```

## Download sample Database
```
https://www.sqlitetutorial.net/sqlite-sample-database/
or 

wget https://cdn.sqlitetutorial.net/wp-content/uploads/2018/03/chinook.zip

Install Unzip
sudo apt install unzip

UNZIP the file
unzip chinook.zip

Delete the source
sudo rm chinook.zip
```

## Create directory
```
mkdir models
mkdir database
```

## Endpoints
```
//GET
localhost:8000/api/playlists
localhost:8000/api/playlists/:id
localhost:8000/api/tracks/:id
localhost:8000/api/artists
localhost:8000/api/artists/:id
localhost:8000/api/albums/:id
```

## POSTMAN (CREATE, UPDATE and DELETE)
Note: this endpoints is post type
```
//UPDATE
//POST: localhost:8000/api/artists/
//Body (raw)
{
    "id": 2,
    "name" "Acceptable"
}

//CREATE
//POST: localhost:8000/api/create/artists
//Body (raw)
{
    "name" "New artist"
}
```

Note: this endpoint is direct function
```
//DELETE
localhost:8000/api/playlists/:id
```
# BeenRed
Reddit-like site built with Node.js, Express, Sequelize, Jasmine, PostgreSQL, EJS, CSS, and Bootstrap.


![Landing Screenshot](https://i.imgur.com/wltUpxx.jpg)

## About
BeenRed was a project that was part of my Bloc Mentorship Program curriculum. We were tasked with building a functioning Reddit-like site using the Agile process and with only user stories given to us.


![Main Screenshot](https://i.imgur.com/ReGGccm.jpg)
![Topic Page Screenshot](https://i.imgur.com/xHd8I8p.jpg)

## Setup
Running Locally
Make sure you have [Node.js](https://nodejs.org/en/) and [PostgreSQL](https://www.postgresql.org/) installed.

Download and install dependencies.
```
git clone git@github.com:darccide/BeenRed 
cd BeenRed
npm install
```

Check that src/db/config/config.json is setup like below (You may need to change your "username" and "password" depending upon your local setup) and make sure that Postgres is running:
```
{
	"development": {
		"username": "postgres",
		"password": null,
		"database": "blocipedia-dev",
		"host": "127.0.0.1",
		"dialect": "postgres",
		"logging": false,
		"operatorsAliases": false
	},
	"test": {
		...
	},
	"production": {
		...
	}
}
```

Init and seed database :
```
sequelize db:migrate
sequelize db:seed:all
```

Run the project :
```
npm start
```
Your app should now be running on localhost:3000.


## Built With
* [Node](https://nodejs.org/en/)
* [Express](https://expressjs.com/)
* [PostgreSQL](https://www.postgresql.org/)
* [Passport](http://www.passportjs.org/)
* [Bootstrap](https://getbootstrap.com/)
* [EJS](https://ejs.co/)
* [Jasmine](https://jasmine.github.io/)

## Author
Steven Thomson is a Fullstack Developer who currently resides in South Korea, but is transistioning back to the U.S. If you would like to contact him:

 * steven.thomson88@gmail.com
 * [Steven Thomson's LinkedIn](https://www.linkedin.com/in/steventhomson1988/)

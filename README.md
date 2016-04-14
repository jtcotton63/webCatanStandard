# BYU CS340 Settlers of Catan

This is a web game that allows four players to play the Settlers of Catan game.

## Run
Run the server using the ant target 'server'

`ant server`

## Play
Locate the dashboard at `http://localhost:8081/index.html`
Click login.html
Register, create a game, and have fun

## To Run the Server
ant clean
ant jar-web-server

java -jar web-server.jar <port-num> <num-saves> <data-wipe> <storage>
	port-num: Default is 8081
	num-saves: number of changes in state. default is 50.
	data-wipe: reset the persistent storage devices. Possible values are true or false.
	storage: Values are file, mongo, sqlite


Web version originally cloned from https://github.com/reedcwilson/catan
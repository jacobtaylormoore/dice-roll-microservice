# dice-roll-microservice
Implementation of the dice roll microservice RESTful API. This API allows POST calls returning pseudorandom dice rolls. The body of the call should specify the number of dice requested to roll (numDice) and the number of faces per die (numFaces). 

## Setup
Clone this repository: 
```
git clone https://github.com/jacobtaylormoore/dice-roll-microservice.git
```

### Dependencies 
Be sure you have Node and Node Package Manager:
https://nodejs.org/en/download/

To download the latest version of npm: 
```
npm install -g npm
```
Or to check your version 
```
npm -v
```

This application also uses express: 
```
npm install express
```
and cors: 
```
npm install cors
```

## Run 
The server is set to run on Port 8080. You may change this by adjusting the local constant PORT if necessary. 

To run, in your terminal enter: 
```
node diceroll.js
```

### Example call

POST http://localhost:8080/dice HTTP/1.1
Content-Type: application/json

{ 
    "numDice": "3" 
    "numFaces": "20"
}
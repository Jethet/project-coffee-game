# ironhack-first-project
# GET YOUR COFFEE


## Description

GET YOUR COFFEE is designed for the true coffee lover who will not accept sub-standard quality like McBrownWater or Starbrew Diluted Stuff. Lemonade and alcohol, or something like tea, are out of the question. The true coffee lover only wants the best: top-quality five-star golden guaranteed high standard coffee!

GYC challenges the player to carefully watch the line-up of beverages, and immediately press the space bar as soon as the Best Coffee cup moves under the coffee machine. If done correctly, the player earns a cup of coffee. If the player forgets to click when the Best Coffee cup passes under the coffee machine, the coffee cup moves off the screen and the player's score is reduced by one. 

If the player gets down to a count of zero coffee cups, the game is over. The speed of the beverage moving across the screen can be increased or decreased. Once the speed is below 0, no beverages will enter the screen anymore.

The player can play for a maximum time of one minute, and after that the game is over. There are some disgusting sounds to accompany the player's game.


## MVP
The line-up of beverages are moving from right to left at a certain speed. The type of beverage is randomized.

There is a counter to keep track of the number of coffee cups scored. There is also a counter that keeps track of the time. On the Game Over screen there is an option to play the game again.


## Backlog
Two of the three options that were listed as backlog items have been created and implemented:

* speed-o-meter
  The speed is shown in the header bar, next to the plus (+) button.

* increase speed to make game more challenging
  The speed of the movement of the beverages can be increased with the plus (+) button and decreased with the minus (-) button.
  
* Extra functionality: sounds have been added for the movement on the gamescreen and for the space click.  

The third backlog item remains.
* save player's results in an overview

Another extra feature could be adding movement to the bialetti coffee maker, and make the game even more difficult.


## Link to GitHub Pages for this project
https://jethet.github.io/ironhack-first-project/

## Data structure
#### main.js


buildSplashScreen(){  
}

buildGameScreen(){  
}

buildGameOverScreen(){  
}



#### game.js

Game(){  
  this.canvas;  
  this.ctx;  
  this.time;  
  this.score;  
  this.beverage;  
}

Game.prototype.start = function(){  
}

Game.prototype.startLoop = function(){  
  this.clearCanvas()  
  this.updateCanvas()  
  this.updateGameStatus()  
}

Game.prototype.checkScreenCollision = function(){  
}

Game.prototype.updateScore = function(){  
}

Game.prototype.setGameOver = function(){  
}

Game.prototype.checkCoffeeClicked = function(){  
}

Game.prototype.checkTime = function(){  
}

Game.prototype.printTime = function(){  
}


#### beverage.js

Beverage(){  
  this.size;  
  this.direction;  
  this.speed;  
  this.x;  
  this.y;  
  }
  

Beverage.prototype.draw = function(){  
}

Beverage.prototype.moveForward = function(){  
}



### States and States Transitions

- splashScreen()
  - buildSplash()
  - addEventListener(startGame)
  
  
- startGame()
  - create new Game()
  - game.start()
  - addEventListener(checkCoffeeClicked)
  
  
- gameOver()
  - buildGameOver()
  - addEventListener(startGame) 

### Tasks

    Main - buildDOM
    Main - buildSplashScreen
    Main - addEventListener  (start)
    Main - buildGameScreen
    Main - buildGameOverScreen
    Game - buildCanvas
    Game - clearCanvas
    Game - updateCanvas
    Game - drawCanvas
    Game - setGameOver
    Game - checkScreenCollision
    Game - createBeverage
    Game - beverage.moveForward
    Game - addEventListener  (press spacekey)
    Game - addEventListener  (play again)
    
    

### [Trello link: click here](https://trello.com/b/ihmt0jKI/ironhack-first-project-get-your-coffee)

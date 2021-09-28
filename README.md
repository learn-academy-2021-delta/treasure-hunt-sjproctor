# React Treasure Hunt Game

### Remember:
- Pseudocode!!
- Ask clarifying questions

### User Stories
- As a user, I can see a page with a 3 by 3 grid board game with a question mark in each square. (done)
  - branch: board-game
  - added a div to square with styling
  - imported Square to App
  - mapped over the array in state and returned the Square component call
  - wrapped a div around the mapped components logic
  - styled the gameboard using flexbox
  - added styles to the square to make the question mark larger and centered
- As a user, when I click on one of the question marks an alert appears with the index position of that question mark in the array. (done)
  - branch: alert-index
  - create an onClick in the square div
  - create a handler method for the square div
  - passed index as props to square
  - create a handleGamePlay method to act as a functional prop
  - passed the handleGamePlay to Square
- As a user, when I click on one of the question marks instead of the alert the question mark turns into a tree emoji.
  - branch: tree-emoji
  - destructured board out of state
  - updated the particular value to a tree emoji
  - emoji keyboard: control + command + spacebar
  - setState after manipulating the array
- As a user, if I select the winning square the question mark will become a treasure emoji and if I select the losing square the question mark will become a bomb emoji.
  - branch: treasure-bomb
  - added treasure and bomb locations to state
  - added a componentDidMount to create random numbers
  - set the state values of treasure and bomb to the random numbers
  - create a conditional that looks at the location of the treasure and bomb compared to the location of the click
  - else return a tree 
- As a user, I can see a counter that shows how many guesses I have left. The counter starts at 5 and decrements one every time I click on a square that is not the treasure nor the bomb.
- As a user, I can see a message informing me that I won the game if I select the square that contains the treasure.
- As a user, I can see a message informing me that I lost the game if I select the square that contains the bomb.
- As a user, I cannot continue to play the game after I win or lose.
- As a user, I can see a message informing me that I lost the game when I run out of turns (the counter reaches zero).
- As a user, I can click on a “Play Again” button that will restart the game.

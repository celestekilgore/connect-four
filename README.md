# connect-four

HTML structure:
    -gameboard div parent element (container)
    -have an eventListener for clicks
        -child nested div elements
        -7 wide, 6 deep (7th top row for clicking)
        
Represent a played-piece
    -finding the lowest/last square with no color change

JavaScript
    -utilize nested arrays for the in-memory game board


Flow of game
    -toggle color so that every turn alternates b/w blue and red


Function names/descriptions
    -createBoard()
        -creates a blank starting board
    -handleClick()
        -find the lowest square in that column that doesn't have a color, add color circle to that square
    -checkTurnColor()
        -toggle between red/blue each click
    -checkForFourInARow()
        -check to see if any four circles of the same color are adjacent (vertically, horizontally, or diagonally)
        -lock gameboard
    -wonGame()
        -lock gameboard
        -'you win'

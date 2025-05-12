# Assignment-5-Slider-Puzzle-Game-solution

Download Here: [Assignment 5 Slider Puzzle Game solution](https://jarviscodinghub.com/assignment/assignment-5-slider-puzzle-game-solution/)

For Custom/Original Work email jarviscodinghub@gmail.com/whatsapp +1(541)423-7793

In this assignment, you will build a slider puzzle game from scratch. The purpose is to become familiar with event handling for various window components.

(1) Slider Puzzle Game

You will be creating the following application:

This application represents a slider puzzle game. There are 15 tiles that can be exchanged horizontally or vertically with a blank tile in order to shuffle the image pieces around. When the tiles are arranged in the correct order, they form a complete image and the game is done. The game is timed … so the faster you can complete the puzzle, the better your score.

The game must meet all of the following requirements:

There is a 4 x 4 grid of 16 Buttons that will hold the images for a puzzle. Your interface should show these buttons as indicated in the screen snapshot above. Each button should be 187 x 187 pixels in size. With a 1 pixel spacing vertically and horizontally between each button. You will need to set the padding to 0 for each button using setPadding(new Insets(0,0,0,0));
This will allow the image to take the full space in the button. There are 4 sets of images available for you to use (although you can add your own as well). These are available on the course website, where you downloaded the assignment. All images must be unzipped and copied into the src folder of this assignment in order to be able to be loaded properly. For each puzzle, there are 17 images … one is a thumbnail image which shows the whole image in 187×187 size. The others are the individual tile images (each 187×187 in size) and are labeled with the format Name_RC … where Name is the name of the puzzle (i.e., Pets, Scenery, Lego or Numbers) and R is the row number and C is the column number for that image (i.e., 0, 1, 2 or 3). Recall that you set the image for a button as follows: 

setGraphic(new ImageView(new Image(getClass().getResourceAsStream(filename)))); where filename is a string representing the name of the file (e.g., “Lego_21”). It may be a good idea to make sure that you can create the buttons and display all of the images from a puzzle in order on each button before you go any further on the assignment.

Your GUI should also show the complete image (i.e., use the available Thumbnail image) as a Label and underneath it should be a ListView showing (at least) the names of the 4 puzzles. See snapshot above. 
There should be a
Start/Stop button (shown as Stop on the snapshot above) as well as a “Time:” Label and a TextField that shows the time that has elapsed since the puzzle was started. All components must be

“nicely” arranged/sized with reasonably consistent margins all around.

Upon window startup, the buttons should show the png image on
each button, the thumbnail Label should be enabled and the Start button should be DARKGREEN with

WHITE letters indicating “Start”. The time should be “0:00”. See image here. 

When an item is selected from the list, the appropriate image should be shown in the Thumbnail Label.
When Start is pressed, the game should begin running. When the game is running, the following should happen:
The Thumbnail Label should be disabled (it will look faded as in the first snapshot on this assignment).
The Start button should become DARKRED and indicate “Stop” instead of “Start”.
The images on the buttons should be changed to the 16 images for the tiles that make up the puzzle image. One of these tiles (chosen randomly) should remain as a blank one. The tiles should be shuffled randomly (see first snapshot) … more will be mentioned about this below.
A Timer should be started. Use a Timeline object (from the animation package). Here is how to set up the timer to tick once per second. You should set this up in the start() method:
updateTimer = new Timeline(new KeyFrame(Duration.millis(1000), 

new EventHandler

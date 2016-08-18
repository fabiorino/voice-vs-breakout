# Your Voice vs Atari Breakout
Move the paddle with your voice just by using two different sounds: a sound will make it go right, the other one will make it go left.

#### YouTube video:
[![ScreenShot](http://i.imgur.com/3Ksirj9.png)](https://www.youtube.com/watch?v=AeUyKfJJpM0)

# Source Code
### Overview
There are three packages in this project. The game and the audio engine are independent of each other. The main package is the "link" between them.

### Packages
- **main**: it contains the main function. Its job is to create a "link" between the game and the audio engine. A loop continuously reads the current frequency and chooses if the paddle has to be moved to the right, to the left or it shouldn't be moving.
- **breakout**: contains the Atari Breakout game. You could take this package and use it as a standalone game with simple code modifications.
- **audioengine**: contains the function that allows to get the current frequency of the sound from the microphone. 
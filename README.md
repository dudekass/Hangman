# Hangman

Language: Python 
Development environment: VS Code 
total time spent on challenge: 3h45min

All code herein is original and do not contain other people's solution, nor artifical intelligence usage.


## Game Description

The user has to guess a word randomly drawn from a list of 10 words, but has to enter letter by letter in order to do so. There is no maximum attempts allowed, you may play again as many times as you want. The user should only guess one letter at a time, and should only input valid letters.
At the end of the game, once you find out what the word is, the game will tell you how many guesses it took you to discover the word. 


## Features

- Randomly selects a word from a predefined list of words.
- Displays the guessed letters and tracks incorrect guesses.
- Ends the game when the player guesses the word
- It has no maximum number of incorrect guesses


## Requirements

- **For Windows Users**: Download the `.exe` file and run the game without needing Python installed.
- **For macOS Users**: Dowload the 
- **For Python Source Code Users**: Python 3.x and the following dependencies are required:
  - `random` (part of Python’s standard library, no installation needed)


## Running the Game

1. **Download the Executable**:
   - Download the `hangman_game.exe` file from the repository or your provided source.

2. **Run the Game**:
   - Double-click `hangman_game.exe` to open the game in a terminal window.
   - Follow the prompts to guess letters and play the game.


## Thought Process

I had many ideas regarding how to approach this challenge, I first utilized the approach of using different functions for each part of the challenge, and later put them all together in a while loop. It didn't work out, I started to have some problems with the loops and functions. My second approach was to utilize only on function and within it call different variables and make the entire game run based on this. However, it also did not work out. I did get a better feeling when approaching the challenge in this way, because I was able to randomly choose the word to be guessed with the same while loop used to discover the word, which made it easier to restart the game with a randomly different word. I did have conflicts with the welcoming part, and the word list as well, which made me try a third and final approach. In my final approach, I decided to treat the welcoming part of the game as a function, and the actual part of the game as another. The welcome function was very easy to do, what took me some time was the game function. I started by the while loop that would be responsible for each new game played. Then, the first part was to randomly choose a word, figure out its length (how many letters it had), set the correct amount of underscores to be guesses, set the counts to zero, and let the player know how many letters there were to their word. The second part was related to input that the User was going to do. I needed to make sure that the input was in fact a single, valid, and non-repeated letter. After setting up the basic information regarding the guess, I worked on the actual "Hangman" part of the code, which was seeing if the letter was present in the word, its position, and to create a database cointaing the user's guesses. After doing so, I focused on the way each information was going to be displayed at the user's terminal. Then, finally, I got to the part where the user guesses the entire word correctly. As instructed and in the "Rules & Requirements" page, we should offer to the User the option to play again, and so I did. When the player discovers the word, the while loop breaks and enables the program to choose a random word again, and to restart the game. At the very end of my code, I call the both the welcome and game functioins, so that it can in fact play in the User's terminal when they install it.

## Unfinished Work

I did not have the chance to actually draw a person hanging and that's due to two main reasons: lack of knowledge, and lack of time. The total amount of time I spent with the code alone was around 2hours and 30 minutes, after doing so I spent around 1 hour making the .exe file and that's because I personlly wrote my code using a macOS, and no one in my household uses windows. I first tried to use brew and wine in my own terminal and computer, but it took me a long time and didn't work out. I was able to find a 2021 hp computer at home, but it also took a while for it to start. Then, I downloaded Python and VS Code on it, and was able to use "pyinstaller" to convert the file into an .exe and uploaded it to github. Now regarding the lack of knowledge, I can certainly understand the logic behind adding a new body part every time there's a wrong guess, but I was not able to actually do a "drawing" that looked like a man being hanged, and the body parts didn't quite align themselves in a clear and understanding way. Therefore I chose to focus on the code per si, and make sure that at least that was in the way I wanted and with no errors. 



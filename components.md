QUESTIONS: 1. What does the component need? 2. What is your responsibility? 3. What things change during the component's execution?

GuessLetters

1. A function that stores a word (in a hidden way at the beginning), receives the letters pressed and needs a useState to change the different types of className, one for when the letter is checked and another one for when it is empty.
2. It checks the letter received through the button and if the letter matches one of the hidden word it paints it and shows it to the user.
   If the letter does not match the state remains empty and does not change.
3. It changes its state from empty to full when the letter is guessed.

Hangman

1. A function to find out if the previous turn has missed the letter. It needs 11 different types of states through className to paint them on the screen when the user fails.
2. It paints the result if the user fails and advances one state at a time, to paint the picture of the hangman, also when the game reaches its last state it sends the information to the Result component.
3. It changes its visual state in the hangman drawing through the 11 different className types.

Letters

1. It needs to store all the letters of the alphabet and to receive the clicked letter in each moment through the onClick event.
2. Sends the clicked letter and paints it to the UsedLetters component and the GuessLetters component if applicable.
3. Deactivates the letter if it is selected but visually has no change for the user.

Result

1. Need a function to know if the game is finished by receiving a response from GuessLetters or Hangman.
2. Receive the final status of Hangman in case of losing the game or the status of GuessLetters in case of winning, and show the user the result.
3. Change the message on the screen depending on whether we win or lose the game.

UsedLetters

1. It needs an empty initial state and as it receives the used letters it stores them.
2. Store the letters preventing them from repeating and paint them on the screen to show them to the user.
3. Change their length as letters are added.

App

1. Need all the child components to call their functions and store the array of words to play with.
2. It structures the web and the game, and evaluates if the letter is successful or failed. It acts as a link between the different components.
3. It changes what the user can see.

# Wordle BASIC
Wordle BASIC is a [Wordle](https://www.powerlanguage.co.uk/wordle/) clone implemented entirely in TI-84+CE BASIC. No external libraries or dependencies are required.

## Installation
Download and ungroup WORDLE.8xo into RAM to install. Note the size of the group (~60 kb) as this much free RAM is required to play.

## Gameplay
Your aim is to guess a hidden 5-letter word in six tries or less, using information about previous guesses to inform your next.
Enter words using the keypad, with `DEL` to backspace and `2ND`/`ENTER` to submit a guess. If the word is invalid, a red `!` will flash.

After submitting a valid guess, the letters of the guess will be colored according to how they align with the secret word.
A *green* letter is in the correct position, an *orange* letter is correct but not in the right spot, and a *grey* letter does not appear anywhere.

Orange letters respect the frequency of a letter in the secret word. That is, if there are two or more of the same letter in a guess, the later instances will be colored *only* if that many letters also appear in the secret word. For example, if the secret word is SCANT and you guess FUNNY, the first N will be grey and the second will be green.

## Stats
The game tracks how many guesses you take to guess the secret word, as well as your current win streak. To reset your stats, run `ClrList thetaWD`.

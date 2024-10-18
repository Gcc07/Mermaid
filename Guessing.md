# Guessing Game
This is a flowchart representing the logic that would be seen in a Guessing Game where a computer generates a number from 1 - 10.

```mermaid
flowchart TD
Start([Start]) --> 1[Machine Chooses Number 1 - 10]
1[Machine Chooses Number 1 - 10] --> 5[Ask User For Input]
5[Ask User For Input] --> id1[\Person Inputs Guess\] 
id1[\Person Inputs Guess\] --> 4[Input is bad]
4[Input is bad] --> 5[Ask User For Input]
id1[\Person Inputs Guess\] --> 2[Guess Is Incorrect]
id1[\Person Inputs Guess\]--> 3[Guess Is Correct]
2[Guess Is Incorrect] --> 1[Machine Chooses A Number From 1-10]
3[Guess Is Correct] --> id2{Ask To Play Again} 
id2{Ask To Play Again} --> 7[No]
id2{Ask To Play Again} --> 8[Yes]
7[No] --> End([End])
8[Yes] --> 1[Machine Chooses A Number From 1-10]

```
The logic of this game is as follows: 
You start. The computer chooses a number between one and ten, and asks for your guess. You input a guess, and depending on your answer the following can happen.
1. You are correct.
2. You are incorrect.
3. You have incorrectly input an answer (syntax.) 

If you are correct, the computer asks to play again. You can choose to play again, which will send you to the beginning, or end then and there.
If you are incorrect, you are prompted to answer again.
If your input is bad, you are promted for input again.
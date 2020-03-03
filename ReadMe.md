# Snooker Scoring

This is just a simple project that can take some basic commands/key-strokes and produce a fully functional scoring system for a game of snooker.

This was just a little experiment I had the idea to attempt after attending a few snooker tournaments and seeing the electronic scoring system in action.

## Notation

The program uses as simple a notation as possible, I admit I'm stealing some of this off of the existing scoring system used by the World Snooker Tour. The notation is as follows:

- Setting up a game:
  - **P:[player]** -> Sets up the player, with [player] being their name.
  - **Fr:[n]** -> Sets up the total frames being played, with [n] being the value.
- During a game:
  - **C** -> Starts/Stops the current Frame clock, signalling the start of the frame/match.
  - **P** -> Pass to next player, for when the player does not pot.
  - **1..7** -> Represents the point value of the ball potted.
  - **F:[n]** -> Signals that a foul was committed, with [n] being it's value.
  - **EoF** -> Signals the end of the current frame.
  - **EoM** -> Signals the end of the current match.

The notation is imputted by the user using their keyboard, and if I feel like it later a GUI. The result of the input will look like a ticker tape which can be exported and replayed to view the results of the match, with the potential for frame-by-frame breakdowns, highest break, and potentially even average shot times, pot success, etc.

An example of a game could look like this (the program will automatically add the delimiters):

{P:Alice;P:Bob;Fr:11;C;P;P;1;7;F:4;.....;EoF;EoM}

For a 11 frame game between Alice & Bob, with Alice going first.

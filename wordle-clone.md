# Wordle Clone

Quick example of a [Wordle](https://www.nytimes.com/games/wordle/index.html) clone for pair-programming exercises.

## Word List

For a cleaned list of valid words, check out [this Gist](https://gist.github.com/benmurden/3774e011a3739856b14d079add764e75).

## About this task

- Should ideally take about 40 minutes to complete in a pair-programming scenario
  - The current Node.js example took about 20 minutes to do
- Could expand this repo to include examples in other languages

## Task requirements

Write a Wordle clone in any language you like. Don't worry too much about presentation, just take some input and return some output. You could expand it to be a CLI application, or even a full web page if you want to get fancy.

### Wordle rules

- The player will try to guess a valid 5 letter word from the English language
- Each guess will show the player how close they are to the correct word
  - Tell the player which letters were correct and in the right place
  - Tell the player which letters were in the word, but in the wrong place
  - Tell the player which letters were not in the word
- Repeat letters in the guess should consider repeat letters in the answer
  - Every letter over the number of repeats should show as not in the word
  - For each repeat letter in the answer show appropriate guess information
- How you determine this and what the output should be is up to you!

### Example I/O
| Guess | Answer | Output | Text      |
|-------|--------|--------|-----------|
| spice | spice  | 🟩🟩🟩🟩🟩  | G,G,G,G,G |
| brand | spice  | ⬛⬛⬛⬛⬛  | N,N,N,N,N |
| epics | spice  | 🟨🟩🟩🟩🟨  | Y,G,G,G,Y |
| pipes | spice  | 🟨🟨⬛🟨🟨  | Y,Y,N,Y,Y |
| ladle | jolly  | 🟨⬛⬛🟩⬛  | Y,N,N,G,N |

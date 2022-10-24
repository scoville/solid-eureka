# Wordle Clone

Build a quick [Wordle](https://www.nytimes.com/games/wordle/index.html) clone for your programming exercise!

## Word List

For a cleaned list of valid words, check out [this Gist](https://gist.github.com/benmurden/3774e011a3739856b14d079add764e75).

## Task requirements

Write a Wordle clone in any language you like. Don't worry too much about presentation, just take some input and return some output. You could expand it to be a CLI application, or even a full web page if you want to get fancy.

We don't expect you to necessarily finish the task.

### Wordle rules

- The player will try to guess a valid 5 letter word from the English language
- Each guess will show the player how close they are to the correct word
  - Tell the player which letters were correct and in the right place
  - Tell the player which letters were in the word, but in the wrong place
  - Tell the player which letters were not in the word
- Repeat letters in the guess should consider repeat letters in the answer
  - Every letter over the number of repeats should show as not in the word
  - For each repeat letter in the answer show appropriate guess information
- How you determine this, and what the output should look like, is up to you!

### Example I/O

The outputs shown here are examples and your program need not necessarily produce the exact same output format, as long as it can be read and understood.

For example:
- 🟩 = Letter is in the word and in the correct place.
- 🟨 = Letter is in the word but in the wrong place.
- ⬛ = Letter is not in the word.

| Guess | Answer | Output | Text      |
|-------|--------|--------|-----------|
| spice | spice  | 🟩🟩🟩🟩🟩  | G,G,G,G,G |
| brand | spice  | ⬛⬛⬛⬛⬛  | N,N,N,N,N |
| epics | spice  | 🟨🟩🟩🟩🟨  | Y,G,G,G,Y |
| pipes | spice  | 🟨🟨⬛🟨🟨  | Y,Y,N,Y,Y |
| ladle | jolly  | 🟨⬛⬛🟩⬛  | Y,N,N,G,N |

# Flashcard
Small flashcard programm

FlashCard v2.0.2
Jonathan Rosenthal, Frédéric Vogel, Eric Mink

## Compilation
The program has to be compiled using the C++11 standard.

`g++ -std=c++11 -Wall FlashCard.cpp -o FlashCard`

## Execution
The program is executed by calling ./FlashCard in the same directory as the program.
It can either be called with the name(s) of flashcard files as arguments or without. If called without
the program will ask for the name of the flashcard file, which must be in the same directory.

Additionally, `--version` may be passed as an argument with or without accompanying flashcard files. However, do not pass `--version` multiple times!

## Flashcard File
The flashcard file contains n flashcards in the following manner:
- On the (2*i)-th line, delimited by '\n', the front of the i-th card.
- On the ((2*i)+1)-th line, delimited by '\n', the back of the i-th card.
  The following symbols have special meaning:
- `\n`: Delimits the front from the back from the front and so on
- `|`:  Delimits a new line *inside* of the card
- `$`:  Delimits a tab character *inside* of the card
- Any line starting with `//` will be ignored (since v 2.0.2)

The symbols '|', '$' and '\n' also break the flow of the proram, requiring the user to type in enter to continue
the execution.

## Closing
Just press Ctrl+c


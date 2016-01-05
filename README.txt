Jotto is a word game that is very similar to Mastermind. In this version, the computer will choose a five-letter word called the 
"target". It must be in a dictionary, must not be a proper noun (a name), and must not be a contraction (like “isn't”). It may contain
repeated characters.

An example is displayed on the right. The target word is "MYTHS".

Words	Exact	Partial
N	Y	M	P	H	1	2
Q	U	A	K	E	0	0
P	Y	G	M	Y	1	1
P	S	Y	C	H	0	3
M	Y	T	H	S	5	0

The player then repeatedly guesses words in an attempt to guess the target word. The guesses must conform to the same rules as the 
target: in the dictionary, five letters, not a proper noun, may contain repeated characters. After each guess the computer will 
indicate two values: the number of exact matches and the number of partial matches. An exact match is where target[i] = guess[i] (ie. 
correct letter and position). A partial match is where target[i] = guess[j], i ≠ j (ie. correct letter, incorrect position). Exact 
matches are found before partial matches and a given letter participates in at most one match. Note the 'Y's in "PYGMY", for example. 
One approach to counting might be to replace characters that have already been matched with a non-alphabetic character.

The game ends when either the player quits, guesses the target, or runs out of guesses (typically 10).


How to use:
	1. Use "make ARGS="TARGE" command. Using the second method, you can 
	   set the target word by passing the additional argument.(Without 
	   the additional argument, the target word will be generated 
	   automatically.)
	2. Use "make" command to compile and run the program.
	3. In the file menu, you could use "New Game" to start a new game.
           Use "Quit", you could quit the program.
        4. You have 10 chances in total. Once you have used up 10 chances,
           the game is over.

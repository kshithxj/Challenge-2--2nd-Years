
# SOSC Round 2 challenge — 2nd Years

Problem 1
I read the direction values and rotated each grid row by 1 step.
R means rotate right and L means rotate left.  
After doing this for all rows, I took the middle row (floor(n/2))
and added the ASCII values of each character.  
This sum became Clue 1.

Problem 2
I reversed the input string, then removed every 3rd character.
After that I shifted each remaining character by +2 in ASCII.
From the new string I counted all vowels (a, e, i, o, u).
This count became Clue 2.

Problem 3
Based on the description:
- prime numbers go straight to the final state,
- even numbers reach the final state eventually,
- odd composite numbers do not move.

I checked each number with this rule and counted how many end in the
terminal state. That became Clue 3.

Final Key
Clue 1 was converted to hexadecimal.
Then Clue 2 was repeated Clue 3 times.
Format: <hex_of_clue1>-<clue2_repeated>

Final Key: 181-4444444

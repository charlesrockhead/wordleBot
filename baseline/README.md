# Baseline model

baseline model:
1. Initialize set of words W to the entire wordle bank
2. Guess a random word in W, call it w
3. Based on the game response to the guess w, limit our set of words W to words that match the response (i.e. if we got a green letter, limit our search to words which have the same letter in the same spot. if we got a yellow letter, limit our search to words which have the letter in any spot.)
4. Repeat steps 2 and 3 until we have the correct guess, or until we have used 6 tries.

Note that 3 will likely require some more complex logic for words with double letters, etc.

potential improvements:
- Guess starting words which have letters with high frequency in the English language (rather than just a random initial word). This may help us get more info from our first guess.
- Rather than randomly guessing words from our set W at any point in time, maybe we can build some sort of distribution over the words W and guess randomly using that distribution. Of course, this is what a probabilistic model would do. So, this is more of an extension.

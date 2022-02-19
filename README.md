# wordleBot
conquer wordle

the plan:
- Get the wordle word bank. We can get this from the site's JavaScript. Then we can use this word bank to guide our searches (is this cheating lol??). Wordle's word bank is just all 5 letter words minus the ones that people don't know (they surveyed people).
- Code up the Wordle game so we can test.
- simple baseline model: guess randomly from the set of words which match our current restrictions
- from there, we can improve. I'm sure we can formulate some simple probabilistic model to tell guide our search better than random. Will think once we see baseline performance and what types of words we may have issues with.

Goal: 3 guess average (I imagine that the baseline won't do this lol)

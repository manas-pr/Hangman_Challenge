# Hangman_Challenge

Description of my deployed strategy:

•	My approach follows a statistical method. Initially, I assign a count of one to the most frequently occurring letter in a word. This approach ensures that if a letter appears multiple times in the word, each instance is considered separately. I preprocess the word by eliminating spaces from the input, then search for words with similar letter patterns in a dictionary. From this, I infer the highest occurring letter that hasn't been guessed in the current round.
•	Subsequently, I calculate the ratio of vowel count to word length. If the ratio exceeds 55%, it's statistically improbable (based on distribution patterns) for additional vowels to be present.
•	When similar words cannot be found in the provided dictionary for the partially guessed word, I emulate human reasoning by attempting to divide the word into smaller components (prefixes/suffixes). This strategy aims to determine the most suitable letter by referring to a secondary dictionary containing substrings derived from the original word list.
•	Lastly, if the letter isn't found in the substring dictionary, the algorithm makes an educated guess by selecting the most frequently used letter across all words that hasn't been guessed yet.
•	The resulted accuracy is 56% 

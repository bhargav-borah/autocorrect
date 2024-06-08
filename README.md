# autocorrect

## Autocorrect Implementations

This repository contains two Python implementations of autocorrect systems:

### 1. Minimum Edit Distance Autocorrect

This system suggests corrections for misspelled words by calculating the minimum number of operations (insertions, deletions, replacements) required to transform one word into another. It uses dynamic programming to compute the minimum edit distance between two words.

#### Features:

- **Minimum Edit Distance Calculation:** Utilizes dynamic programming to compute the minimum edit distance between two words, supporting operations such as insertions, deletions, and replacements.
  
- **Vocabulary-based Suggestions:** Given a vocabulary, suggests corrections for misspelled words by finding the closest words based on edit distance.
  
- **Efficient Algorithm:** Suitable for small to medium-sized vocabularies.

### 2. Probabilistic Autocorrect with Two Edits

This system suggests corrections by allowing at most two edits to the misspelled word. It chooses edits that actually occur in the vocabulary and have the maximum probability of occurrence in the vocabulary.

#### Features:

- **Two Edit Maximum:** Allows up to two edits (insertions, deletions, replacements) to the misspelled word.
  
- **Probabilistic Selection:** Edits are chosen based on their occurrence in the vocabulary and their probability of occurrence.
  
- **Efficient Selection:** Optimized for performance by focusing on likely corrections.

## Dependencies:

- Python 3.x
- NumPy library (for matrix operations)

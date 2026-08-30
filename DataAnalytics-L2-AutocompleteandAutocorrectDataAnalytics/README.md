# Level 2 - Task 5: Autocomplete and Autocorrect Data Analytics

## Objective

Analyze the efficiency and accuracy of autocomplete and autocorrect algorithms using Natural Language Processing (NLP) techniques.

The project implements frequency-based n-gram autocomplete models and an edit-distance-based autocorrect system.

## Tech Stack

- Python
- Pandas
- NumPy
- NLTK
- Matplotlib
- Seaborn
- Jupyter Notebook
- Levenshtein Distance

## Dataset

A large text corpus was created using multiple Project Gutenberg books available through the NLTK Gutenberg corpus.

The selected texts included:

- Jane Austen's *Emma*
- Jane Austen's *Persuasion*
- Jane Austen's *Sense and Sensibility*
- Shakespeare's *Hamlet*
- King James Bible

### Corpus Statistics

| Metric | Result |
|---|---:|
| Characters | 6,521,824 |
| Original Tokens | 1,188,562 |
| Clean Tokens | 612,650 |
| Unique Words | 21,310 |

## NLP Preprocessing

The following preprocessing techniques were applied:

- Lowercasing
- Tokenization
- Punctuation removal
- Alphabetic word filtering
- Stopword removal

## Autocomplete

Two frequency-based n-gram models were implemented.

### Bigram Model

The bigram model predicts the next word using the current word as context.

### Trigram Model

The trigram model predicts the next word using the previous two words as context.

The autocomplete system was tested on at least 10 input prefixes and the top three predictions were displayed.

## Autocomplete Performance

| Model | Precision | Recall | Top-3 Accuracy |
|---|---:|---:|---:|
| Bigram | 0.0949 | 0.2846 | 0.2846 |
| Trigram | 0.3102 | 0.9307 | 0.9307 |

The trigram model significantly outperformed the bigram model because it uses two previous words and therefore has more contextual information.

## Autocorrect

A custom Levenshtein-distance algorithm was implemented because the `pyspellchecker` package could not be installed in the Kaggle environment.

Levenshtein distance measures the minimum number of character-level insertions, deletions, and substitutions required to transform one word into another.

The system was tested on 20 deliberately misspelled words.

### Autocorrect Results

| Metric | Result |
|---|---:|
| Test Words | 20 |
| Correctly Corrected | 12 |
| Incorrectly Corrected | 8 |
| Accuracy | 60.00% |
| Precision | 60.00% |
| Recall | 60.00% |
| F1-Score | 60.00% |

## Visualizations

The notebook contains:

- Top 20 most frequent words
- Bigram autocomplete results
- Trigram autocomplete results
- Bigram vs Trigram performance comparison
- Autocorrect correction results
- Autocorrect confusion matrix
- Autocorrect performance metrics
- Algorithm comparison

## Key Findings

1. The trigram model achieved a Top-3 accuracy of **93.07%**, substantially higher than the bigram model's **28.46%**.

2. Using additional context significantly improved autocomplete performance in this corpus.

3. The Levenshtein-based autocorrect system correctly corrected **12 out of 20** deliberately misspelled words, achieving **60% accuracy**.

4. Some spelling errors were incorrectly mapped to common words with similar edit distances, demonstrating the limitations of using character similarity alone.

## Limitations

The implemented algorithms are simplified compared with production systems such as Google Keyboard.

Major limitations include:

- Limited contextual understanding
- Dependence on corpus frequency
- Data sparsity for unseen word combinations
- No personalization
- No sentence-level semantic understanding
- Levenshtein distance only considers character-level similarity
- Common words may be selected even when they are inappropriate in context
- No keyboard-layout or typing-error information
- No neural language model
- Smaller training corpus than commercial systems

## Conclusion

This project demonstrates the practical use of NLP techniques for autocomplete and autocorrect.

The bigram and trigram models showed that additional linguistic context can significantly improve next-word prediction. The trigram model achieved a Top-3 accuracy of 93.07%.

The custom Levenshtein-distance autocorrect system achieved 60% accuracy on 20 deliberately misspelled words.

Although these approaches are useful for demonstrating fundamental NLP concepts, production systems require larger datasets, contextual language models, personalization, and additional signals to achieve high-quality predictions and spelling corrections.

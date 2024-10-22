# Part-of-Speech (POS) Tagger

This project implements a POS tagging system using the Brown Corpus and the Viterbi algorithm with optimizations for unknown words. The system predicts the POS tags for a given sentence and provides a web interface for users to input sentences and view the predicted tags.

## Demo Video

[Click here to watch the demo video](demo.mp4)

## Features

- **Viterbi Algorithm**: Optimized for unknown words using smoothing techniques.
- **Cross-Validation**: Evaluates performance using 5-fold cross-validation, reporting accuracy, confusion matrix, and per-tag accuracy.
- **Gradio Interface**: Provides an easy-to-use web interface for users to input sentences and get POS tags in real-time.
- **Corpus**: Uses the Brown corpus from the NLTK library, with the universal tagset.


## Evaluation

The model uses a 5-fold cross-validation to evaluate its performance. Metrics reported include:

- **Accuracy**: The average accuracy across folds.
- **Confusion Matrix**: To visualize true vs. predicted POS tags.
- **Per POS Tag Accuracy**: Accuracy for each POS tag (ADJ, VERB, NOUN, etc.).

## Web Interface

The project includes a Gradio-based web interface for easy interaction.


### Example Input:
**Sentence**:  
`The quick brown fox jumps over the lazy dog.`

### Example Output:
[('The', 'DET'), ('quick', 'ADJ'), ('brown', 'ADJ'), ('fox', 'NOUN'), ('jumps', 'VERB'), ('over', 'ADP'), ('the', 'DET'), ('lazy', 'ADJ'), ('dog', 'NOUN')]


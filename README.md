# Autocorrect System

This project implements a simple autocorrect system using Python. The system suggests corrections for misspelled words based on a predefined vocabulary and word probabilities. It uses an algorithm to generate possible edits of a word and selects the most probable correction based on word frequency data.

## Features

- **Edit Distance Calculation**: The system generates candidate words within an edit distance of 1 or 2 from the input word.
- **Vocabulary Matching**: It checks the candidate words against a predefined vocabulary.
- **Probabilistic Correction**: The system selects the most likely correct word based on word probabilities derived from frequency data.

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/UllekhPatel/Autocorrect-Model.git
   cd Autocorrect-Model
   ```

2. Install the required Python packages:

   The project primarily uses Python's standard library, so no external dependencies are required. However, if your project evolves to include external packages, you can install them using pip. Here is an example command to install common packages (adjust as needed for your project):

   ```bash
   pip install numpy pandas
   ```

   *(Note: If you later add dependencies, you can list them in a `requirements.txt` file or directly install them using pip.)*

## Usage

1. Run the Jupyter notebook:

   ```bash
   jupyter notebook autocorrect.ipynb
   ```

2. Follow the instructions in the notebook to input a word and receive suggested corrections.

## Functions

- `edit1(word)`: Generates all possible edits that are one edit distance away from the input word.
- `edit2(word)`: Generates all possible edits that are two edits away from the input word.
- `correct_spelling(word, vocabulary, word_probabilities)`: Suggests corrections for the input word based on the vocabulary and word probabilities.

## Example

When you input a word like `"botes"`, the system may suggest corrections like:

```plaintext
[('notes', 7.220129721664e-05), ('bones', 2.4067099072213332e-05), ('bote', 1.2033549536106666e-05), ('boxes', 1.2033549536106666e-05), ('votes', 1.2033549536106666e-05)]
```

The system will then select the most probable correction, for example, `"notes"`.

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request for any enhancements or bug fixes.

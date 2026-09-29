# Word Frequency Counter

A small Python program that counts how often each word appears in a piece of
text. It is designed as a beginner-friendly example of functions,
conditionals, dictionaries, recursion, and loops.

## Table of contents

- [Features](#features)
- [Requirements](#requirements)
- [Getting started](#getting-started)
- [Using the counter](#using-the-counter)
- [How it works](#how-it-works)
- [Getting help](#getting-help)
- [Contributing](#contributing)
- [Maintainer](#maintainer)

## Features

- Prompts for text directly in the terminal.
- Treats uppercase and lowercase versions of a word as the same word.
- Removes commas, periods, exclamation marks, and question marks before
  counting.
- Returns an empty dictionary for empty input.
- Uses a dictionary to report each word and its frequency.

## Requirements

- Python 3
- No third-party packages

## Getting started

1. Clone this repository and change into its directory:

   ```bash
   git clone https://github.com/VoidLance/course-files-python-word-frequency-counter.git
   cd course-files-python-word-frequency-counter
   ```

2. Run the program:

   ```bash
   python3 "Word Frequency Counter.py"
   ```

3. Enter text when prompted. For example:

   ```text
   Enter a text: Python is fun. Python is useful!
   python: 2
   is: 2
   fun: 1
   useful: 1
   ```

The output preserves the order in which each word first appears.

## Using the counter

The main function is `count_word_frequency(text)`. It accepts a string and
returns a dictionary mapping each word to its count:

```python
frequency = count_word_frequency("red blue red")
print(frequency)
# {'red': 2, 'blue': 1}
```

For reuse in another program, move or copy the function into a Python module
whose filename can be imported normally. The function returns `{}` when
`text` is empty:

```python
count_word_frequency("")
# {}
```

## How it works

1. Empty input is handled immediately.
2. The text is lowercased and selected punctuation is removed.
3. The text is split into words.
4. A recursive helper updates a frequency dictionary for each word.
5. The program prints each word and its count.

## Getting help

For questions or suspected bugs, [open an issue](https://github.com/VoidLance/course-files-python-word-frequency-counter/issues)
with the Python version, command used, input text (if safe to share), and
observed output. You can also review the source in
[`Word Frequency Counter.py`](./Word%20Frequency%20Counter.py).

## Contributing

Contributions are welcome. To propose an improvement:

1. Create a fork and make a focused change.
2. Verify the program manually with representative inputs.
3. Open a pull request describing the change and how it was checked.

Please keep changes focused, use clear Python, and update this README when
usage or behavior changes.

## Maintainer

This project is maintained by [VoidLance](https://github.com/VoidLance).

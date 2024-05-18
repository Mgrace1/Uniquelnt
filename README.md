# Integer File Processor

This Python script reads integers from an input file, filters out those not within the range of -1023 to 1023, sorts the remaining unique integers, and writes them to an output file.

## Features

- Reads integers from a text file.
- Filters integers to include only those within the range of -1023 to 1023.
- Ensures all integers are unique.
- Sorts the unique integers in ascending order.
- Writes the sorted integers to an output text file.

## Requirements

- Python 3.x

## Usage

1. Place your input file with integers in the same directory as the script, or specify the correct file path.
2. Run the script using Python.
3. The output file will be created in the specified directory with the sorted unique integers.

## Function Description

### `process_file(input_file_path, output_file_path)`

This is the main function of the script.

#### Parameters:

- `input_file_path` (str): The path to the input text file containing integers.
- `output_file_path` (str): The path to the output text file where sorted unique integers will be written.

#### Example:

```python
process_file("input.txt", "output.txt")
#### Examples:
Suppose you have an input file sample_input.txt with the following content
100
-50
2000
1023
-1023
apple
50
-50
100
Running the script with process_file("sample_input.txt", "output.txt") will produce an output file output.txt with the following content:
-1023
-50
50
100
1023

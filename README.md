# Pascal/CamelCase to Snake_Case Converter

This Python program converts strings written in PascalCase or camelCase into snake_case. It's a simple utility function that ensures proper formatting by following a consistent naming convention.

## Features

- **Convert PascalCase to snake_case**: Automatically inserts underscores (`_`) before uppercase letters and converts them to lowercase.
- **Convert camelCase to snake_case**: Handles camelCase strings in the same way.
- **Ignores leading/trailing underscores**: The function removes unwanted underscores from the result.

## Code Overview

### `convert_to_snake_case(pascal_or_camel_cased_string)`
This function converts a PascalCase or camelCase string into a snake_case string.

- `pascal_or_camel_cased_string`: The input string to convert.
- Returns: A `snake_case` formatted string.

#### Algorithm Steps:
1. Iterate through each character in the input string.
2. For uppercase characters, prepend an underscore (`_`) and convert the character to lowercase.
3. For lowercase characters, append them to the result as is.
4. Join the list of characters into a single string and remove leading/trailing underscores.

### `main()`
Provides an example usage of the `convert_to_snake_case` function.

- Prints the converted version of a sample PascalCase string (`IAmAPascalCasedString`).

## Example Usage

```python
def main():
    print(convert_to_snake_case('IAmAPascalCasedString'))
    # Output: i_am_a_pascal_cased_string
# Contract Errors

This Solidity contract demonstrates various error-handling mechanisms and custom error declaration.

## Overview

This contract provides three functions (`e1`, `e2`, `e3`) demonstrating different error handling approaches in Solidity. Additionally, it defines a custom error `UserDefError` and includes a function `myError` that utilizes it.

## Details

### Function `e1(uint a)`

- **Purpose**: Multiplies input by 2 if it's greater than 10.
- **Error Handling**: Uses `require` statement to check if input is greater than 10. Throws an error message if the condition fails.

### Function `e2(uint a)`

- **Purpose**: Doubles the value of state variable `b` if input is less than or equal to 10.
- **Error Handling**: Utilizes `revert` statement with a custom error message if input is greater than 10.

### Function `e3(uint a)`

- **Purpose**: Raises `b` to the power of 2 and asserts that input is 0.
- **Error Handling**: Uses `assert` statement to verify the condition. If not met, transaction will revert.

### Custom Error `UserDefError`

- **Purpose**: Defines a custom error with two parameters: `z` (uint256) and `message` (string). Used for more specific error handling.

### Function `myError(uint256 a)`

- **Purpose**: Checks if the gas limit exceeds a certain threshold.
- **Error Handling**: Throws a custom error `UserDefError` if gas limit exceeds the specified threshold.

## License

This project is licensed under the terms of the MIT license.
For queries contact : negikartik025@gmail.com

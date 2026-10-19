# Infix to Postfix Visualizer

## About the Project

The Infix to Postfix Visualizer is a web-based application that demonstrates how an infix expression is converted into a postfix expression using a stack. It shows the conversion process step by step, making it easier to understand the working of stack operations and operator precedence.

The project is designed for students who are learning Data Structures and Algorithms.

## Features

- **Infix to Postfix Conversion:** Converts infix expressions into postfix expressions.
- **Step-by-Step Visualization:** Shows how each token is processed.
- **Stack Visualization:** Displays the operators stored in the stack and highlights the top element.
- **Postfix Output:** Displays the output as the conversion progresses.
- **Step Controls:** Move backward, forward, play automatically, or finish the conversion.
- **Animation Speed:** Adjust the speed of the visualization.
- **Example Expressions:** Includes sample expressions to help users understand different cases.
- **Input Validation:** Displays error messages for invalid expressions and mismatched brackets.
- **Conversion Trace:** Provides a table showing each step, the action performed, the stack, and the output.
- **Time and Space Complexity:** Explains the efficiency of the conversion algorithm.

## Technologies Used

- HTML
- CSS
- JavaScript

No external libraries or frameworks are required.

## How to Run the Project

1. Download or clone this repository.
2. Open the project folder.
3. Locate the HTML file.
4. Open the HTML file in any modern web browser.
5. Enter an infix expression and click **Convert expression**.

You can also use Visual Studio Code with the Live Server extension to run the project locally.

## How to Use

1. Enter an infix expression in the input field.
2. Click **Convert expression**.
3. Click **Next step** to see the next operation.
4. Use **Back** to view the previous step.
5. Click **Play** to run the animation automatically.
6. Adjust the animation speed using the speed slider.
7. Click **Finish** to complete the conversion.
8. Check the step-by-step trace table to understand how the stack and output change.

## Supported Operators

| Operator | Description | Precedence |
|---|---|---|
| `^` | Exponentiation | Highest |
| `*` | Multiplication | Medium |
| `/` | Division | Medium |
| `+` | Addition | Lowest |
| `-` | Subtraction | Lowest |

The application supports parentheses `()`, square brackets `[]`, and curly braces `{}` for grouping expressions.

Exponentiation is right-associative, while the other supported operators are left-associative.

## Example

**Infix Expression:**

```text
A+B*(C-D)^E/F
```

**Postfix Expression:**

```text
A B C D - E ^ * F / +
```

The conversion uses a stack to temporarily store operators and brackets while operands are added directly to the postfix output.

## Algorithm

1. Scan the infix expression from left to right.
2. Add operands directly to the postfix output.
3. Push opening brackets onto the stack.
4. When a closing bracket is encountered, pop operators until the matching opening bracket is found.
5. For each operator, compare its precedence with the operator at the top of the stack.
6. Pop operators with higher precedence and equal precedence when the current operator is left-associative.
7. Push the current operator onto the stack.
8. After scanning the expression, pop all remaining operators into the output.

## Complexity Analysis

- **Time Complexity:** O(n)
- **Space Complexity:** O(n)

Here, `n` represents the number of tokens in the expression.

## Purpose

This project helps students understand infix-to-postfix conversion, stack operations, operator precedence, associativity, and algorithm complexity through an interactive visual demonstration.

## License

This project is available for educational and learning purposes.
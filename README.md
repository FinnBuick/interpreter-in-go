# Monkey Programming Language Interpreter

A Go implementation of the Monkey programming language interpreter from [Writing An Interpreter In Go](https://interpreterbook.com/) by Thorsten Ball.

## About

This interpreter includes:
- Lexer
- Parser
- Evaluator
- REPL (Read-Eval-Print Loop)

The Monkey language supports:
- Integers, booleans, strings
- Arrays and hash maps
- Functions and closures
- Basic arithmetic operations
- Variable bindings

## Running the REPL

```bash
go run src/monkey/main.go
```

Example:
```monkey
>> let add = fn(x, y) { x + y };
>> add(5, 5);
10
```

## Project Structure
```
src/monkey/
├── ast/          # Abstract Syntax Tree
├── evaluator/    # Tree-walking evaluator
├── lexer/        # Lexical analyzer
├── object/       # Object system
├── parser/       # Recursive descent parser
├── repl/         # Interactive shell
├── token/        # Token definitions
└── main.go       # Entry point

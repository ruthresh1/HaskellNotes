# HaskellNotes
Notes for Haskell Programming language

### Introduction
Haskell is a programming language that uses purely Functional Programming Paradigm. In purely functional languages, a function has no side-effects. It is statically typed, lazy language, which promotes referential transparency. It treats programming as a series of transformations on data.

### Important Note
Install stack to practice haskell in your local or cloud system
Follow instructions
https://docs.haskellstack.org/en/stable/README/

### Stack
Basic stack usage
```code
// Starting a new project
$ stack new my-project
$ cd my-project
$ stack setup
$ stack build
$ stack exec my-project-exe

// To launch a repl
$ stack ghci
$ stack repl
```

### Strings
A set of characters enclosed within double quotes
```haskell
Prelude> :type 'a'
'a' :: Char
Prelude> :type "Hello!"
"Hello!" :: [Char]

-- Printing
Prelude> print "Hello"
// "Hello"
Prelude> putStrLn "Hello"
// Hello
//
Prelude> putStr "Hello"
// Hello


-- A simple haskell program print1.hs
module Print1 where
main :: IO ()
main = putStrLn "hello"

Prelude> :l print1.hs
Prelude> main
hello
```

### Functions
A function is a set of repeatable instructions, that is invoked as and when needed.
It has a name and accepts parameters as needed, to return a value
```haskell
Prelude> succ 1
// 2
Prelude> min 1 2
// 1
Prelude> max 1.2 2.4
// 2
```

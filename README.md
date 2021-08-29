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
```haskell
Prelude> :type 'a'
'a' :: Char
Prelude> :type "Hello!"
"Hello!" :: [Char]
```

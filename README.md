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
```bash
# Starting a new project
$ stack new my-project
$ cd my-project
$ stack setup
$ stack build
$ stack exec my-project-exe

# To launch a repl
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
"Hello"
Prelude> putStrLn "Hello"
Hello
Prelude> putStr "Hello"
Hello


-- A simple haskell program print1.hs
module Print1 where
main :: IO ()
main = putStrLn "hello"

Prelude> :l print1.hs
Prelude> main
hello
```

String concatenation
Concatenate means to join
Two ways to do them for strings is using '++' and concat function
```haskell
Prelude> name = "Ruthresh" ++ " Kumar"
Prelude> putStr name
Ruthresh Kumar

Prelude> first_name = "Ruthresh"
Prelude> last_name = " Kumar"
Prelude> name = concat first_name last_name
Prelude> putStr name
Ruthresh Kumar
```

### Functions
A function is a set of repeatable instructions, that is invoked as and when needed.
It has a name and accepts parameters as needed, to return a value
```haskell
Prelude> succ 1
2
Prelude> min 1 2
1
Prelude> max 1.2 2.4
2
```

Functions in Haskell default to prefix syntax, meaning that the function being applied is at the beginning of the expression rather than the middle. Operators are functions which can be used in infix style. All operators are functions.
Functions can use ' as part of function name.

### Control statements
#### if else
In haskell if statement should always have a corresponding else.
```haskell
Prelude> doubleSmallNumber x = if x > 100 then x else x*2   
Prelude> doubleSmallNumber 2
4
```

### Lists
A homogeneous grouping of elements.
```haskell
Prelude> let lostNumbers = [4,8,15,16,23,42]  
Prelude> lostNumbers  
[4,8,15,16,23,42]
Prelude> [1,2,3,4] ++ [9,10,11,12]  
[1,2,3,4,9,10,11,12] 

-- List operations

```

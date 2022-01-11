# Introduction

## What is Haskell?

---

Haskell is a purely functional programming language, meaning that it's a bit different from your usual imperative programming languages.

For starters, haskell's variables are immutable and constant. When you have set a variable to 5, it will always be 5.

Haskell also has no side effects. When you pass in the same parameters to a function, it should always return the same output.

Another feature of Haskell is that it is _lazy_. Unless specifically told otherwise, it won't execute functions _until_ it needs to show you a result. With this in mind, you can create sequences ranging from 1 to infinite, and the compiler won't complain.

Haskell is statically typed. It's just saying that for every variable declaration you have to assign a specific type to it (it can handle type inference, but the type will still be static). More on this [here](https://www.haskell.org/tutorial/goodies.html).

## Setting Up Your Environment

---

The most widely used compiler for Haskell is called GHC, short for Glasgow Haskell Compiler. The GHC also has an interactive mode, which lets you to interact with your scripts in real time.

To install GHC, you can head on to [here](https://www.haskell.org/ghc/download.html).

## Using Your Environment

---

Haskell files are created with .hs file extensions. Now there are two ways to use GHC and execute your haskell files:

### Compiler Mode (GHC)

> More details [here](https://downloads.haskell.org/ghc/latest/docs/html/users_guide/usage.html)

To compile a file, you just need to run `:l yourfile.hs`, this is an example:

```bash
$ ghc helloworld.hs
$ ./helloworld
Hello, World!
```

### Interactive Mode (GHCi)

> More details [here](https://downloads.haskell.org/ghc/latest/docs/html/users_guide/ghci.html)

With the interactive environment, you can load and test haskell files in real-time, without compiling.

First, you have to be in GHCi

```shell
$ ghci
GHCi, version 8.y.z: https://www.haskell.org/ghc/  :? for help
ghci>
```

To load a file, you just need to run

```ghci
:l helloworld.hs
```

After changing things in your file, you can reload with `:l yourfile.hs` again, or use

```ghci
:r
```

which reloads the current loaded file.

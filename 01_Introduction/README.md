[<< Back](../README.md)

#Introduction to FP, Reactive, and Scala

## Principles of functional programming

Functional programming favors state management and immutability in a declarative programming way.

When you are coding in functional programming, you tend to use fewer variables, for loops, and etc. and write more functions and make function compositions.

### Core principles of functional programming

#### Immutability

Once you assign a value to something, that value won't change.

You will create another instance or another pointer to that instance, but you won't change that variable's value.

This makes your code parallel by nature.

#### Disciplined state

When you are coding with functional programming principles in mind, you avoid, as much as possible, having a shared mutable state.

Of course you can have state, but you should keep it local, which means inside your function.

#### Pure functions and no side effects

Pure functions are those with no side effects.

Side effects can be database call, global variables, IO call, and so on.

#### First-class functions and higher-order functions

With first-class functions, you can pass functions as arguments to other functions and to return values as functions.

Higher-order functions often means language support for partial functional application and currying.

Currying is a technique to transform a function with multiple parameters in a sequence of functions with each function having a single argument.

#### Type systems

The compiler helps in making sure that you only have the right types as arguments, turn statements, function composition, and so on.

One of the biggest benefits of the strong type system is that you have to write fewer tests, because the compiler will take care of several issues for you.

## Scala REPL

```
$ scala

scala> "Hello World"
res0: String = Hello World”
```

Scala is a hybrid language, which means it is object-oriented and functional as well.

### Scala object-oriented HelloWorld program

```
scala> object HelloWorld {
     |   def main(args:Array[String]) = println("Hello World")
     | }
defined object HelloWorld
scala> HelloWorld.main(null)
Hello World
scala>
```

We used the word `object` instead of `class`.
`Object` is a `singleton` in Scala.

Next we see the word `def` that is used in Scala to create functions.

When we extend from Scala class App, we perform inheritance and we don't need to define the main function. (less code)

```
scala> object HelloWorld extends App {
     |  println("Hello World")
     | }
defined object HelloWorld
scala> HelloWorld
object HelloWorld
scala> HelloWorld.main(null)
Hello World
scala>
```

## Scala Language the basics

### Scala variables

* `var`: The value can change - this is ok for local variables.
* `val`: The value is immutable - try to use this as much as possible.

#### Common types

`Int`, `Double`, `Boolean`, and `String`.

#### Implicit typing

```
scala> val x = 10
x: Int = 10
scala> val y = 11.1
y: Double = 11.1
scala> val b = true
b: Boolean = true
scala> val f = false
f: Boolean = false
scala> val s = "A Simple String"
s: String = A Simple String
scala>
```

#### Explicit typing

```
scala> val x:Int = 10
x: Int = 10
scala> val y:Double = 11.1
y: Double = 11.1
scala> val s:String = "My String "
s: String = "My String "
scala> val b:Boolean = true
b: Boolean = true
scala>
```

### Scala conditional and loop statements

[<< Back](../README.md)

> Declarative programming is a programming paradigm that expresses the logic of a computation without describing its control flow.

> Imperative programming is a programming paradigm that uses statements that change a program’s state.

> Declarative Programming is like asking your friend to fix your car. You don’t care how to fix it, that’s up to her.

> Imperative Programming is like your friend calling your father that tells her how to fix your car step by step.

<hr/>

> From GeeksforGeeks

### Difference Between Imperative and Declarative Programming

<table><thead><tr><th><p style=text-align:center>Imperative Programming<th><p style=text-align:center>Declarative Programming<i><strong> &nbsp;</strong></i><tbody><tr><td>In this, programs specify how it is to be done. &nbsp;<td>In this, programs specify what is to be done. &nbsp;<tr><td>It simply describes the control flow of computation.&nbsp;<td>It simply expresses the logic of computation. &nbsp;<tr><td>Its main goal is to describe how to get it or accomplish it. &nbsp;<td>Its main goal is to describe the desired result without direct dictation on how to get it. &nbsp;<tr><td>Its advantages include ease to learn and read, the notional model is simple to understand, etc. &nbsp;<td>Its advantages include effective code, which can be applied by using ways, easy extension, high level of abstraction, etc. &nbsp;<tr><td>Its type includes procedural programming, object-oriented programming, parallel processing approach. &nbsp;<td>Its type includes logic programming and functional programming. &nbsp;<tr><td>In this, the user is allowed to make decisions and commands to the compiler. &nbsp;<td>In this, a compiler is allowed to make decisions. &nbsp;<tr><td>It has many side effects and includes mutable variables as compared to declarative programming. &nbsp;<td>It has no side effects and does not include any mutable variables as compared to imperative programming. &nbsp;<tr><td>It gives full control to developers that are very important in low-level programming. &nbsp;<td>It may automate repetitive flow along with simplifying code structure.&nbsp;</table>
<hr/>

> From StackOverflow

### What is the difference between declarative and imperative paradigm in programming?

Declarative vs. Imperative

A programming paradigm is a fundamental style of computer programming. There are four main paradigms: imperative, declarative, functional (which is considered a subset of the declarative paradigm) and object-oriented.

- **Declarative programming** : is a programming paradigm that expresses the logic of a computation(What do) without describing its control flow(How do). Some well-known examples of declarative domain specific languages (DSLs) include CSS, regular expressions, and a subset of SQL (SELECT queries, for example) Many markup languages such as HTML, MXML, XAML, XSLT... are often declarative. The declarative programming try to blur the distinction between a program as a set of instructions and a program as an assertion about the desired answer.

- **Imperative programming** : is a programming paradigm that describes computation in terms of statements that change a program state. The imperative programs can be dually viewed as programming commands or mathematical assertions.

- **Functional programming** : is a programming paradigm that treats computation as the evaluation of mathematical functions and avoids state and mutable data. It emphasizes the application of functions, in contrast to the imperative programming style, which emphasizes changes in state. In a pure functional language, such as Haskell, all functions are without side effects, and state changes are only represented as functions that transform the state.

The following example of imperative programming in MSDN, loops through the numbers 1 through 10, and finds the even numbers.

```cs
var numbersOneThroughTen = new List<int> { 1, 2, 3, 4, 5, 6, 7, 8, 9, 10 };
//With imperative programming, we'd step through this, and decide what we want:
var evenNumbers = new List<int>();
foreach (var number in numbersOneThroughTen)
{    if (number % 2 == 0)
    {
        evenNumbers.Add(number);
    }
}
//The following code uses declarative programming to accomplish the same thing.
// Here, we're saying "Give us everything where it's even"
var evenNumbers = numbersOneThroughTen.Where(number => number % 2 == 0);

```

Both examples yield the same result, and one is neither better nor worse than the other. The first example requires more code, but the code is testable, and the imperative approach gives you full control over the implementation details. In the second example, the code is arguably more readable; however, LINQ does not give you control over what happens behind the scenes. You must trust that LINQ will provide the requested result.

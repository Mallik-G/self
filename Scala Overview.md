## Scala Overview

- **Scala** is a programming language that integrates the object oriented and functional language features. 

  [![Scala-Programming](https://cdn.journaldev.com/wp-content/uploads/2015/03/Scala-Programming-450x200.png)](https://cdn.journaldev.com/wp-content/uploads/2015/03/Scala-Programming.png)

  ### Scala and Java

- Scala programming language has a wonderfully continental ring to its name, as befits its origins at the École polytechnique fédérale de Lausanne (EPFL) in Lausanne, Switzerland. The Scala logo represents a circular stairway, which may lead you to believe its origin is the term La Scala, meaning a staircase or ladder in Italian, or that it derives from the famous Italian opera house Teatro alla Scala. In fact the name Scala is an abbreviation of the term SCAlable LAnguage, a fitting description of its intention. Professor Martin Odersky and his group at EPFL created the language in 2003 to provide a high-performance, concurrent-ready environment for functional programming and object-oriented programming on the Java Virtual Machine (JVM) platform.

- Scala stands for Scalable Language

- Scala was designed by Martin Odersky.

- Scala was officially released for java platform in early 2004.

- Scala is an object-oriented and functional programming language.

- Scala is modern multi paradigm and hybrid programming language.

- Scala integrates the features of object-oriented and functional languages.

- Scala is designed express common programming patterns in a concise, elegant, and type-safe way.

- Scala designed inspired by Java and Lisp.

- Scala is a strong static type language.

- In Scala, everything is an object whether it is a function or a number.

- Scala does not have support primitive data types.

- Scala source file having an extension of either .scala or .sc.

- Scala is compiled to run on the Java Virtual Machine (JVM)

- Scala is crisp, productive, interactive, Scalability and Reliability

- Scala is interoperable with Java Library.

- Scala allows development in two ways:
  - Interactive Mode
  - Standalone

- We can use Scala for developing following type of applications.
  - Web applications
  - Enterprise applications
  - Mobile applications
  - Desktop applications
  - Data Analysis applications
  - Utilities and Libraries
  - Streaming Applications
  - Parallel and batch processing applications
  - etc...

- Scala is crisp, productive and easy to learn.

- Scala is not extension of Java, but it is interoperable with Java.

- Scala is pure object oriented and functional oriented programming language.

- Scala is a pure object oriented language in the sense that every value is an object

- Scala is pure functional language in the sense that every function is a value.

#### Scala Hello World Progrom:

```scala
Interactive Mode using scala, scala notebook, zeppelin etc...
  
     println("Hello World")
     
Standalone Mode: 
  Step1: example1.scala

      object HelloWorld {
          def main(args:Array[String]) {
             println("Hello World!!")
          }
        }
 Step2: scalac example1.scala // Generates a class file with object name 
 Step3: scala HelloWorld  
 Hello World!!
```

------

## Scala Features:

- Scala is pure Object Oriented
  - Every value is Scala is an Object
  - Functions are also objects 
  - Supports Subclassing
  - Mixin-based composition -- Multiple inheritance
- Scala is Functional
  - In Scala, every function is an object
  - Ananymous Functions
  - Higher- Order functions
  - Nested
  - Currying
- Type inference: Scala offers Type Inference i.e., no need to provide the data type explicitly
- Singleton objects: Scala offers Singleton i.e., no static members.
- Immutability: Scala offers Immutability i.e., can not modify variable values.
- Lazy computation: Scala offers Lazy computation i.e., it evaluates expressions only when they are required.
- Case classes and Pattern matching: Scala case classes are regular classes but there are immutable. Scala case classes are used in combination with Scala pattern matching.
- Concurrency control: Scala provides actor model for better handling of Concurrency.
- String interpolation: Scala String interpolation allows embedding variables as part of Scala string.
- Higher order function: Scala offers high order functions i.e., function takes another function as argument or function returns another function as return value.
- Traits: Scala provides trait which contains fields and methods of type abstract and non abstract.
- Rich collection set: Scala provides a rich set of mutable and immutable collections to manipulate the data.
- Closures: Scala offers ananymous functions
- etc...

------

## Scala Installation:

- Scala requires Java JDK
- Download Java JDK and Install it
- Add JAVA_HOME
- Download Scala based on OS
- Add SCALA_HOME
- Add Scala executables and Java Executables into the System PATH variable in the .bashrc file.

### Checking Scala and Java Installations:

```
 > java -version
 > javac -version
 > scala -version
 > scalac -version

```

## Scala IDEs

- Scala Eclipse (Standalone)
- Scala Shell (Interactive)
- Scala Notebook (Interactive)
- Zeppelin Notebook (Interactive)
- Sublime Text Editor (Standalone)
- Vim/Vi Editor (Standalone)
- InteliJ (Standalone)
- Many more editors

### 1. **HelloWorld using Scala - Standalone**

Let’s break down below snippet. The first thing to notice, is that the whole code is inside an `object` block. Java programmers might find these confusing. Unlike Java, class names need not match with file names, not a big deal but, we do have that freedom here.

Next thing is the strange syntax of `def main()`. To begin with `def` is a keyword to declare methods. There can be arguments for a method and in our case, it is an `Array[String]`. This is similar to Java’s main method, where a string array is an argument to the main method. Can be used for startup config or any runtime variables. This is followed by a `println()` method call which prints statements on to the console. Semicolons are optional in Scala unlike Java and the compiler relies on line breaks to identify the next literal/code block.

```scala
object HelloWorld {
	def main(args:Array[String]) {
		println("Hello World!!")
	}
}
```

Here, **Object** is a singleton object, not a class. **Main** is the usual entry point into the code in Scala. **App** is a trait that can be extended to achieve the same effect

```Scala
object HelloWorldApp extends App {
	println("Helloo world!");
}
```

### 2. HelloWorld using Scala - REPL

Scala provides REPL. The REPL (“Read-Evaluate-Print-Loop”) shell is the interactive mode for running Scala

```Scala
C:\Users\GandhaMa>scala
Welcome to Scala version 2.10.6 (Java HotSpot(TM) 64-Bit Server VM, Java 1.8.0_144).
Type in expressions to have them evaluated.
Type :help for more information.

scala> println("Hello World")
Hello World

```

### 3. Mutable and Immutable Variables

A **variable** is a storage unit in memory that holds data. In Scala, there are two types of variables - 

- **Immutable Variables**: 
  - *val* keyword is used to designate a variable as immutable. 
  - immutable variables once defined, cannot be reassigned 
- **Mutable Variables**: 
  - *var* keyword is used to designate a variable as mutable. 
  - mutable variables can be reassigned

Every ‘variable’ (storage unit) must be declared using one of these keywords

```scala
scala> var radius: Double = 10       // A mutable variable declared using *var*
radius: Double = 10.0

scala> radius = 12                   // A mutable variable can be reassigned a new value
radius: Double = 12.0

scala> radius = "a"                   // A mutable variable cannot be reassigned a new datatype
<console>:8: error: type mismatch;
 found   : String("a")
 required: Double
       radius = "a"
                ^

scala> val PI: Double = 3.14         // An immutable variable declared using *val*
PI: Double = 3.14

scala> PI = 22/7                     // An immutable variable cannot be reassigned a new value   
<console>:8: error: reassignment to val
       PI = 22/7
          ^

```

We have specified datatype Double to both variables. However, specifying the type is optional in Scala. Scala is statically typed language, but has powerful type inference.

***val* or *var* - Why does this distinction matter?**

- Immutability is an important concept in Scala
- Scala encourages the use of immutable variables to drive side-effect free code
- immutable storage units also help keep code safe for concurrent/distributed applications

If you know that a variable’s state should not change once it is assigned - **declare it immutable**. This makes sure that there are no **unintentional** state changes to the variable. It makes maintaining code
far easier. 

### 4. Type Inference - Basics

This is not something unique to Scala, many languages such as OCaml, Haskell, Rust, Swift, C#(starting with version 3.0) already have these.

Let’s start with the [Wikipedia’s definition](https://en.wikipedia.org/wiki/Type_inference).

> Type inference refers to the automatic deduction of the data type of an expression in a programming language

The primary purpose is to help the programmer avoiding verbose typing but still maintaining the compile time type safety of a statically typed language.

> Type inference is the best of both worlds i.e static and dynamic typing.

Or at-least it tries to be. The reality is largely dependent upon where/how we use it.

##### **Overview of a type system**

A type system is a language component that is responsible for type checking.
Scala is a statically typed language, so there are always a defined set of types and anything that does not belong in that set is not regarded as a valid type and an appropriate error is thrown at compile time.

**Why have any type system at all?**

Because computers cannot match human stupidity, and certain things are better handled by the compiler rather than relying on people for getting it right. It also can prevent a ton of bugs that pop up due to improper types. A type system exists to give [type safety](https://en.wikipedia.org/wiki/Type_safety), and the levels of strictness is what differentiates between different languages and run times.

On a high level, because of Scala's Type Inference -

- **Variable types** can often be omitted
- **Function return types** can often be omitted
- **Polymorphic method calls** and **generic class instantiations** can often be omitted

#### Variable types can often be omitted:

In the below code snippet, type is not specified explicitly for *radius*, but Scala's Type Inference sees the value assigned as *10.0* and infers it as a **Double**.

```scala
scala> val radius = 10.0
radius: Double = 10.0
```

In the below snippet, type is not specified explicitly for *radius2*, but Scala's Type Inference sees the value assigned as *10* and infers it as an **Int**.

```scala
scala> var radius2 = 10
radius2: Int = 10
```

In the below snippet, type is specified explicitly for *radius*, Scala's Type Inference sees the value assigned as *10* and would have infer this is an **Int**, but because we specified the type, Scala accepts **Double** as type as it is of higher rank (no loss of precision)

```scala
scala> val radius: Double = 10
radius: Double = 10.0
```

In the below snippet, type is specified explicitly for *radius* as **Int**, but Scala's Type Inference sees the value assigned as *10.0* and would infer this is a **Double**, but because we specified the type as **Int**, Scala throws `error: type mismatch`. Scala will not allow as **Int** is of lower type than **Double** and there could be loss of precision in storing Double values in to an Int.

```scala
scala> val radius: Int = 10.0
<console>:7: error: type mismatch;
 found   : Double(10.0)
 required: Int
       val radius: Int = 10.0
                         ^
```

In the below snippet, type is specified explicitly for *radius* as **Double**, but Scala's Type Inference sees the value assigned as *"10.0"* and would infer this is a **String**, but because we specified the type as **Double**, Scala throws `error: type mismatch`. 

```scala
scala> var radius: Double = "10.0"
<console>:7: error: type mismatch;
 found   : String("10.0")
 required: Double
       var radius: Double = "10.0"
```

**Scala’s follows a combination of sub-typing and local type inference.**

If we notice the error in example below, the compiler is not able to infer/deduce the type of the recursive function. In Scala, we have to annotate the types wherever local type inference does not help. In the second example,  we defined return type of the function and Scala compiled it. 

```scala
scala> def factorial(a:Int) = {
     |     if(a <=1) 1 else a * factorial(a-1)
     |   }
<console>:8: error: recursive method factorial needs result type
           if(a <=1) 1 else a * factorial(a-1)
                                ^

scala> def factorial(a:Int): Int = {
     |     if(a <=1) 1 else a * factorial(a-1)
     |   }
factorial: (a: Int)Int
```

**SubTyping:**

In the below code block, we are constructing heterogeneous lists where sub-typing converts the lower type into a higher type wherever necessary. A simple example would converting an `Int`to a `Double` which is the second example. If it cannot be fit, it goes to the top level i.e the `Any` type. All of this conversion can be translated to the type system hierarchy above.

```scala
scala> List(10, 'a')
res21: List[Int] = List(10, 97)

scala> List(10, 20.0)
res22: List[Double] = List(10.0, 20.0)

scala> List(10, true)
res23: List[AnyVal] = List(10, true)

scala> List(10, "Hello")
res24: List[Any] = List(10, Hello)
```



##### Why does type inference matter?

There are two kinds of programming languages - Statically Typed (Java, C, C++) or Dynamically Typed (Python, JavaScript).

- In Statically Typed Languages, the type of every variable is known at **compile time**, whereas, for Dynamically Typed Languages, the type of every variable is known only at **run time**
- Quick and easy to find bugs as most of them get caught during compile phase itself in statically typed languages, lots of bugs get caught at run time in dynamically typed programming languages 
- In Statically Typed Languages, because of type declarations, code gets verbose, whereas Writing code is quick and fast prototyping is possible in Dynamically Typed Programming Languages.

Scala seeks to get the best of both worlds via **Type Inference**.

Scala is Statically Typed, but it has an elaborate type inference system to guess types. This makes Scala code to look more like a Python code than Java code.



### 5. String Operations

**String concatenation using +**

```scala
scala> val name = "Scala"
name: String = Scala

scala> val greeting = "Hello"
greeting: String = Hello

scala> greeting + name
res1: String = HelloScala

scala> greeting + "\n" + name
res2: String =
Hello
Scala

scala> greeting + " " + name
res3: String = Hello Scala

// You can create multi-line strings using triple quotes """
scala> val complexString = """Scala is
     | an amazing, powerful
     |       programming
     | Languange !!!
     | """
complexString: String =
"Scala is
an amazing, powerful
      programming
Languange !!!
"

```

**String Comparisions**

Unlike in Java, it is safe to compare strings using **==**

```scala
scala> val PI = "pi"
PI: String = pi

scala> val PI2 = "pi"
PI2: String = pi

scala> PI == PI2
res4: Boolean = true

```

We will discuss mainly two things - 

- String Interpolation using **s" "**
- printf notation using **f" "**

**String interpolation using s" "**:

Preface any string with **s** to use string interpolation. Then, that string can contain references to variables prefixed with **$**. Scala will then resolve such variables in the output

```scala
// Referring to variables inside a string 
scala> s"$greeting, $name, How are you today?"
res5: String = Hello, Scala, How are you today?

// You can write an expression in {} which is then computed by Scala
scala> val num = 3
num: Int = 3

scala> s"Three time Two is ${num*2}"
res9: String = Three time Two is 6

// Applying * on strings makes it repeat
scala> s"I am ${name*5}"
res8: String = I am ScalaScalaScalaScalaScala

scala> s"I am ${"sorry"*5}"
res7: String = I am sorrysorrysorrysorrysorry

```

**printf notation using f" "**:

Formatting strings in Scala is easy - preface the string with **f** and you can use the various options provided by **f**. Inside the string, we can refer to variables using **$**, formatter is specified using **%**

```scala
scala> val pi = 3.14159
pi: Double = 3.14159

scala> f"Rounded value of Pi is $pi%.2f"
res10: String = Rounded value of Pi is 3.14
```



### 6. A Unified Type System

Scala's type system is powerful, expressive, and vast. 

**History:** Java's type system is divided between **primitive** types and **reference** types. **Autoboxing** (introduced in Java 1.5) eliminated the need for explicitly casting/converting between primitive types (like int) and their corresponding ('wrapper') reference types (e.g, java.lang.Integer), but there is still an underlying bifurcation of Java's type system -- there is no 'top type' which unifies this split in the type system between primitive and reference types.

Scala has a unified type system. All of Scala’s types, from numbers to strings to collections, exist as part of
a type hierarchy. Every class that we define in Scala will also belong to this hierarchy automatically.

In Scala, all values are instances of a class (no exceptions). But, since Scala runs on the JVM, Scala must show distinction between value and reference types like Java shows. So, Scala, establishes this distinction between value and reference types, by  adding super classes for both reference and value types and a new super class on top of them.

**Diagram:**

The open-headed arrows in the diagram indicate supertypes, a common notation in object-oriented diagrams. The multiple-arrow types at the bottom indicate that they are subtypes of every type in the system, including classes you define on your own. 

![Scala type system](https://madusudanan.com/images/scala-type-system.png)

The Any, AnyVal, and AnyRef types are the root of Scala’s type hierarchy. Any is the absolute root, and all other types descend from its two children, AnyVal and AnyRef. The types that extend AnyVal are known as value types because they are the core values used to represent data.

AnyVal types are accessed just like other types but may be allocated at runtime either on the heap as objects or locally on the stack as a JVM primitive value. 

All other types have AnyRef as their root and are only ever allocated on the heap as objects. The term “Ref ” in “AnyRef ” indicates they they are reference types that are accessed via a memory reference.

Value types are similar to native types in java. They are created as follows.

```
val x : Int = 3
```

While reference types need to have the `new` keyword.

```
val arr = new ArrayBuffer[Int]()
```

Of course there are some exceptions to this. `String` is a special one. Collection classes such as `Array` and `List` have their own `apply` method so that they can be created without the new keyword. Technically, they are objects in the jvm as opposed to native types, so they require the `new` keyword for their creation.

Let us consider 3 functions

```Scala
scala> def printAny(x: Any) = println(x)
printAny: (x: Any)Unit

scala> def printAnyVal(y: AnyVal) = println(y)
printAnyVal: (y: AnyVal)Unit

scala> def printAnyRef(z: AnyRef) = println(z)
printAnyRef: (z: AnyRef)Unit

```

Let us instantiate various values and see how these functions work

```scala
scala> val someVal = 5  // SubType of AnyVal
someVal: Int = 5

scala> val someRef = new Object    // SubType of AnyRef
someRef: Object = java.lang.Object@53ea380b

// printAny will work with either of these values
scala> printAny(someRef)
java.lang.Object@53ea380b

scala> printAny(someVal)
5

// printAnyVal will work with only values and fails for Ref types
scala> printAnyVal(someVal)
5

scala> printAnyVal(someRef)
<console>:10: error: type mismatch;
 found   : Object
 required: AnyVal
Note that implicit conversions are not applicable because they are ambiguous:
 both method any2Ensuring in object Predef of type [A](x: A)Ensuring[A]
 and method any2ArrowAssoc in object Predef of type [A](x: A)ArrowAssoc[A]
 are possible conversion functions from Object to AnyVal
              printAnyVal(someRef)
                          ^
// printAnyRef will work with only Ref types and fails for Value types
scala> printAnyRef(someVal)
<console>:10: error: type mismatch;
 found   : Int
 required: AnyRef
Note: an implicit exists from scala.Int => java.lang.Integer, but
methods inherited from Object are rendered ambiguous.  This is to avoid
a blanket implicit which would convert any scala.Int to any AnyRef.
You may wish to use a type ascription: `x: java.lang.Integer`.
              printAnyRef(someVal)
                          ^

scala> printAnyRef(someRef)
java.lang.Object@53ea380b

```



### 7. Emptiness in Scala

Scala has 6 things that denote emptiness. 

- null
- Null
- Nothing
- Nil
- None
- Unit

**null**: null basically means null as in Java.

A String variable, for example, can be assigned null at any time, such that the variable does not point to any string instance in memory. This assignment of null to a variable declared as type String is acceptable because null is a compatible type for String.

*Reference types can be null, but value types can not.*

```scala
scala> val x: String = null
x: String = null

// Trying to assign null to Value types results in error 
scala> val y: Char = null
<console>:7: error: type mismatch;
 found   : Null(null)
 required: Char
Note that implicit conversions are not applicable because they are ambiguous:
 both method Character2charNullConflict in class LowPriorityImplicits of type (x: Null)Char
 and method Character2char in object Predef of type (x: Character)Char
 are possible conversion functions from Null(null) to Char
       val y: Char = null
                     ^
```

**Null**: 

- Null is a Trait (i.e., a type) not a Value. 
- **Null** is the type for **null**
- Null is a subtype of AnyRef

**Nothing:**

- Nothing is a trait (i.e., a type) not a value

```
scala> val emptyList = List()
emptyList: List[Nothing] = List()

scala> val emptyList = Array()
emptyList: Array[Nothing] = Array()

```

- Nothing can never be instantiated
- Nothing extends everything

**Nil**

- Nil is a special value associated with an empty List
- Nil is a singleton instance of List[Nothing]
- Lists are internally represented as linked lists, and use this special value to signify the end of the list

**None**

- None is a special value associated with an Option

- Option is a (monadic) collection used to capture presence or absence of a value

  ```Scala
  scala> def fraction(numer: Double, denom: Double): Option[Double] = {
       | if (denom == 0) None
       | else Option(numer/denom)
       | }
  fraction: (numer: Double, denom: Double)Option[Double]

  scala> fraction(100,0)
  res32: Option[Double] = None

  scala> fraction(100,10)
  res33: Option[Double] = Some(10.0)

  ```

**Unit**

- Unit is basically like Void in Java

- Unit is the return type of a function that returns nothing, for instance

  ```scala
  scala> def printAny(x: Any) = println(x)
  printAny: (x: Any)Unit

  ```



### 8. Type Operations

Scala provides 4 options to do type operations - 

- asInstanceOf
- isInstanceOf
- to\<Type>
- getClass

**asInstanceOf:** 

Converts the value to a value of the desired type. Causes an error if the value is not compatible with the
new type.

```scala
scala> 124.asInstanceOf[Long]
res34: Long = 124

scala> 123.35.asInstanceOf[Long]
res35: Long = 123

scala> "123".asInstanceOf[Long]
java.lang.ClassCastException: java.lang.String cannot be cast to java.lang.Long
        at scala.runtime.BoxesRunTime.unboxToLong(BoxesRunTime.java:110)
```

**to\<Type>:**

Conversion functions to convert a value to a compatible value.

```scala
scala> 123.toLong
res37: Long = 123

scala> 123.34.toLong
res38: Long = 123

scala> "123".toLong
res39: Long = 123

scala> "abc".toLong
java.lang.NumberFormatException: For input string: "abc"
        at java.lang.NumberFormatException.forInputString(NumberFormatException.java:65)
```

**isInstanceOf:**

Returns true if the value has the given type.

```scala
scala> 123.isInstanceOf[Long]
res41: Boolean = false

scala> 123.34.isInstanceOf[Long]
res42: Boolean = false

scala> 123L.isInstanceOf[Long]
res43: Boolean = true

scala> "123".isInstanceOf[String]
res44: Boolean = true

scala> null.isInstanceOf[String]
res46: Boolean = false

scala> null.isInstanceOf[Null]
<console>:8: error: type Null cannot be used in a type pattern or isInstanceOf test
              null.isInstanceOf[Null]
                               ^

```

**getClass:**

Returns the type (i.e., the class) of a value.

```scala
scala> 123.getClass
res52: Class[Int] = int

scala> 123.toLong.getClass
res53: Class[Long] = long

scala> "123".getClass
res54: Class[_ <: String] = class java.lang.String

scala> List(12,3).getClass
res55: Class[_ <: List[Int]] = class scala.collection.immutable.$colon$colon

```

### 9. Statements v Expressions

Let’s draw a distinction between these two - Scala will make a lot more sense once we do.

**Statements** are units of code that **do not return a value.**

**Expressions** are units of code that **return a value.**

```scala
scala> val radius = 10
radius: Int = 10
```

Here, 10 is an expression. `val radius = 10` is a statement.

In the below statement, `{ val PI = 3.14; PI * radius * radius}` is a code block. The last statement in the block is the return value of the block. 

```scala
scala> val area = { val PI = 3.14; PI * radius * radius}
area: Double = 314.0

```

**Statements v Expressions - Why does this matter?**
Because many constructs that are statements in Java are expressions in Scala. For example - 

- if/else
- for loops
- match

By changing these constructs to expressions (with return values) Scala makes functional programming far easier.  Expressions can be "composed" (chained to each other), but Statements can't. This is the basis for "composition of functions".

### 10 Defining Values and Variables via Expressions

An expression is a unit of code that returns a value. We can take that value and use it to define a variable or a value. 

In the below example, `{ val PI = 3.14; PI * radius * radius}`is an expression which returns `PI * radius * radius`, we used the return value of this expression and assigned it to  new variable `area`.

```scala
val area = { val PI = 3.14; PI * radius * radius}

```

Expressions provide a foundation for functional programming because they make it possible to return data instead of modifying existing data (such as a variable). This enables the use of immutable data, a key functional programming concept where new data is stored in new values instead of in existing variables. Functions, of course, can be used to return new data, but they are in a way just another type of expression.

**Why does this matter?**

**Expressions are "r-values"** which mean that they can be assigned and composed (chained)
**Statements are not "r-values"** - they just sit there and do their thing

By expanding the possible r-values in code, Scala enables functional programming



### 11 Nested Scopes in Expression Blocks

In the below code snippet, we have an expression block nested inside another expression block. The last expression in the outer block is another expression block, so the return value of the inner block is assigned to `area` variable. The expression `PI*radius*radius` from outer scope is ignored.

```scala
scala> val area = {
     |   val PI = 3;
     |   println(s"Inside scope 1, PI = $PI");
     |   PI*radius*radius;
     |   {
     |     val PI = 3.14;
     |     println(s"Inside scope 2, PI = $PI");
     |     PI*radius*radius
     |   }
     | }
Inside scope 1, PI = 3
Inside scope 2, PI = 3.14
area: Double = 314.0
```

**Why does this matter?**

Because **functions** in Scala are merely **named, reusable expression blocks**. if you can have nested expression blocks, you can have nested functions too.

Crucial features in Scala like Nested Functions, First Class Functions, Closures depend on nested scopes in expression blocks.

### 12 IF/ELSE expression blocks

Java, C#, C, C++ have If/Else statements. Scala has If/Else expressions like Microsoft Excel. 

The entire if/else construct is an expression block. The return value of entire block depends on the return value of the boolean expression.

```scala
if (boolean expression) {
    expression block #1
}
else {
    expression block #2
}
```

By the way, an `if` without an `else` will return `Nothing` if the boolean expression evaluates to false

```scala
scala> val numer = 8
numer: Int = 8

scala> val denom = 4
denom: Int = 4

scala> val PI = if(denom != 0) {
     |       numer/denom
     | }
PI: AnyVal = 2

scala> val PI = if(denom != 0) {
     |       numer/denom
     | } else {
     |       None
     | }
PI: Any = 2                              

scala> val denom2 = 0
denom2: Int = 0

scala> val PI = if(denom2 != 0) {
     |       numer/denom2
     | }
PI: AnyVal = ()

scala> val PI = if(denom2 != 0) {
     |       numer/denom2
     | } else {
     |      0.0
     | }
PI: Double = 0.0                         // Type inference  
```

**Why does this matter?**

Java, C#, C, C++ have If/Else statements, Scala has If/Else expressions.

Scala has cleverly transformed If/Else constructs into **r-values**, allowing them to be functionally composed.

```scala
scala> radius * radius * { if(denom != 0) numer/denom else 0.0 }
res58: Double = 200.0
```

### 13 `match` Expressions

Java, C#, C, C++ have switch statements, Scala has `match` expressions, these are actually more powerful, and more widely used than if/else expressions.

- Unlike in Java, only zero or one `case` clauses will evaluate to `true`
- No fall-through, no **break**. There is a  **catch-all** though
- **matches** can be on **value**, but also on **type** and with additional **conditions**

**A value, to be initialized via a match expression**

```scala
scala> val dayOfWeek = "Monday"
dayOfWeek: String = Monday

scala> val typeOfDay = dayOfWeek match {
     |   case "Monday" => "Monday Blues"
     |   case "Sunday" => "Sleepy Sunday"
     | }
typeOfDay: String = Monday Blues

```

Here, `dayOfWeek` is the identifier to be matched, this needs to be defined first. `match` is the keyword, under which we specify a set of cases, of which none or one will be matched. In each case, `=>` is followed by an expression that will be returned if the case is satisfied.

If no case matches, Scala will result in a `Scala.MatchError`.

```scala
scala> val typeOfDay = dayOfWeek match {
     |   case "Monday" => "Monday Blues"
     |   case "Sunday" => "Sleepy Sunday"
     | }
scala.MatchError: Tuesday (of class java.lang.String)
        at .<init>(<console>:8)
```

Match expressions used more widely than if/else statements in Scala - they are a very popular language construct. And that’s why they matter a great deal in Scala (far more than switch statements matter in Java)

### 14 `match` expressions: Pattern guards & OR-ed expressions

There are two ways to add conditions to individual case clauses in a match expression. 

- Pattern guards
- OR-ed expressions

**OR-ed expressions:**

The boolean expressions in a case statement can be OR-ed together

```scala
scala> val dayOfWeek = "Tuesday"
dayOfWeek: String = Tuesday

scala> val typeOfDay = dayOfWeek match {
     |   case "Monday" => "Monday Blues"
     |   case "Sunday" | "Saturday" => "Lazy Weekend"
     |   case "Tuesday" | "Wednesday" | "Thursday" |"Friday" => "Working day"
     | }
typeOfDay: String = Working day

```

**Pattern guards:**

Pattern guards are a way to add an if expression into a case. A pattern guard starts with a placeholder variable called a **value binding**. In this snippet, `someOtherDay` is the value binding variable, which gets value of `dayOfWeek`.  

Pattern guards allow multiple conditions on the same value binding. Only the case where the pattern guard evaluates to true will pass.

```scala
scala> val dayOfWeek = "Sunday"
dayOfWeek: String = Sunday

scala> val typeOfDay = dayOfWeek match {
     |   case "Monday" => "Monday Blues"
     |   case "Tuesday" | "Wednesday" | "Thursday" |"Friday" => "Working day"
     |   case someOtherDay if someOtherDay == "Saturday" => "Sizzling Saturday"
     |   case someOtherDay if someOtherDay == "Sunday" => "Sleeping Sunday"
     | }
typeOfDay: String = Sleeping Sunday

```

**Why does this matter?**

`match` expressions are really important in Scala, and these variants help extend their flexibility a great deal.

### 15 `match` expressions: catchall to match-all

In a pattern matching expression, what if no case matches? It results in a Scala.MatchError. 

We need something like the default case in a switch statement to prevent such errors. Scala offers two options - 

- Value Binding Patterns
- `_` (WildCard Operator Pattern)

**Value Binding Patterns:**

We have already seen Value bindings before, where we use a variable to store the value of the match variable. This variable can then be used in the expression on the right side of the arrow.

In the below snippet, we used `someOtherDay` value binding as a catch all case and wrote an expression

```scala
scala> val typeOfDay = dayOfWeek match {
     |   case "Monday" => "Monday Blues"
     |   case "Tuesday" | "Wednesday" | "Thursday" |"Friday" => "Working day"
     |   case someOtherDay => {
     |     println(s"Some Other Day - Neither a monday nor a working day, its $someOtherDay")
     |     someOtherDay
     |   }
     | }
Some Other Day - Neither a monday nor a working day, its Sunday
typeOfDay: String = Sunday
```



**`_` (WildCard Operator Pattern)**:

Using underscore character `_` as a placeholder is a common theme in Scala. 

> ​	**case _ => expression**

Here, `_` is an unnamed wildcard for the input value. It will match anything. But this placeholder `_` will not work on the right of the => sign. Use it on the left hand side only. On the right side, you can reference the
original match variable.

```scala
scala> val typeOfDay = dayOfWeek match {
     |   case "Monday" => "Monday Blues"
     |   case "Tuesday" | "Wednesday" | "Thursday" |"Friday" => "Working day"
     |   case _ => {
     |     val day = s"Some Other Day - Neither a monday nor a working day, its $dayOfWeek"
     |     day
     |   }
     | }
typeOfDay: String = Some Other Day - Neither a monday nor a working day, its Sunday

```

Attempting to access `_` on the right of the => will result in an error

```scala
scala> val typeOfDay = dayOfWeek match {
     |   case "Monday" => "Monday Blues"
     |   case "Tuesday" | "Wednesday" | "Thursday" |"Friday" => "Working day"
     |   case _ => _
<console>:4: error: unbound placeholder parameter
         case _ => _
                   ^
```

### 16 `match` expressions: down casting with Pattern Variables

In Java, a common use case of nested if statements is to downcast using `instanceof`.
By the way, its a key failing of the Java `switch` statement that it can’t predicate on type. Scala’s `match` is carefully built to test on type of the match variable.

There is a special type of case clause, which tests the type of a variable

> **case \<identifier> : \<Type> => \<expression>**

**Example 1:**

```scala
scala> val radius: Any = 10
radius: Any = 10

scala> val typeOfRadius = radius match {
     |   case radius: Int => "Integer"
     |   case radius: String => "String"
     |   case radius: Double => "Double"
     |   case _ => "Any"
     | }
typeOfRadius: String = Integer

```

**Example 2:** The placeholder **`_`** can be used as the pattern variable.

```scala
scala> val radius: Any = "10"
radius: Any = 10

scala> val typeOfRadius = radius match {
     |   case radius: Int => "Integer"
     |   case _: AnyRef => "String"
     |   case _ => "Any"
     | }
typeOfRadius: String = String

```

**Example 3: A catch-all/match-all:** We can use either a placeholder or a value binding to make sure that some case is always satisfied.

Here, no standard case matches Double, so, catch-all case kicks in.

```scala
scala> val radius: Any = 10.0
radius: Any = 10.0

scala> val typeOfRadius = radius match {
     |   case radius: Int => "Integer"
     |   case radius: String => "String"
     |   case _ => "Any"
     | }
typeOfRadius: String = Any

```

**Example: 4 Type Mismatch:**

The “scrutinee” (variable whose type is matched) must be a base type, else an error will result.

```scala
scala> val radius: String = "10"
radius: String = 10

scala> val typeOfRadius = radius match {
     |   case radius: Int => "Integer"
     |   case radius: String => "String"
     |   case _ => "Any"
     | }
<console>:9: error: scrutinee is incompatible with pattern type;
 found   : Int
 required: String
         case radius: Int => "Integer"
                      ^
```

### 17 `for` loops can be expressions OR statements

For loops can be set up as either statements or expressions by adding or removing just 1 word `yield`. The presence of this word converts a `for` loop into an expression. A for-loop with `yield` will “yield” a collection of the return values of each iteration of the loop.

A for-loop without `yield` will simply execute the iterations without saving their return values.

**for-loop as a statement - nothing will be returned**:

```scala
// Define a simple list of the days of the week
scala> val daysOfWeek = List("Mon", "Tue", "Wed", "Thu", "Fri", "Sat", "Sun")
daysOfWeek: List[String] = List(Mon, Tue, Wed, Thu, Fri, Sat, Sun)

// Iterate over this list and print a message
// Each iteration merely prints a value, and does not return anything
scala> for (day <- daysOfWeek) {
     |   day match {
     |     case "Mon" => println("Monday")
     |     case otherDay => println(otherDay)
     |   }
     | }
Monday
Tue
Wed
Thu
Fri
Sat
Sun

```

**for-loop as an expression - yield is used**:

`for` loop with `yield` allows to perform an operation on a collection in a loop and collects and returns the output of each iteration as another collection.

```scala
// Use yield keyword 
// Change the match expression to return something
// The results of this for-loop are saved in value x
scala> val x = for (day <- daysOfWeek) yield {
     |   day match {
     |     case "Mon" => "Monday"
     |     case otherDay => otherDay
     |   }
     | }
x: List[String] = List(Monday, Tue, Wed, Thu, Fri, Sat, Sun)

```

**`for` loops: 2 types of iterators**

We can iterate a collection in two ways - 

- Value Binding
- numerical range

```scala
// Value Binding
scala> for(day <- daysOfWeek){
     |   println(day)
     | }
Mon
Tue
Wed
Thu
Fri
Sat
Sun

// Numerical range
scala> for(i <- 0 to daysOfWeek.size -1) {
     |   println(daysOfWeek(i))
     | }
Mon
Tue
Wed
Thu
Fri
Sat
Sun

// Scala even has a way to eliminate the clunky “-1”, source of so many off-by-1 errors - until
scala> for(i <- 0 until daysOfWeek.size) {
     |   println(daysOfWeek(i))
     | }
Mon
Tue
Wed
Thu
Fri
Sat
Sun

```

**So which of these is the best way to iterate over a collection?**

Actually none. Scala has powerful aggregate functions such as foreach, map, flatmap. But you should know how to use for loops anyway

### 19 `for` loops with `if` conditions: Pattern Guards

Here is how we would combine an `if` condition with a `for` loop in Scala.

```scala
scala> for(day <- daysOfWeek if day == "Mon") {
     |   println(day)
     | }
Mon
```

Merging the if condition into the for loop makes the code more concise. This is called a “Pattern Guard” in
Scala. 



### 20 Nested `for` Loops: Nested Iterators

Here is how we would set up a nested loop in Scala. Notice that there 2 ranges, without a comma separating them.

```scala
scala> for{i <- 0 to 2
     |     j <- 0 until 1} {
     |   println(s"$i-$j")
     | }
0-0
1-0
2-0

// Its perfectly OK to combine different types of iterators
scala> for{i <- 0 to 1
     |     j <- daysOfWeek} {
     |   println(s"$i-$j")
     | }
0-Mon
0-Tue
0-Wed
0-Thu
0-Fri
0-Sat
0-Sun
1-Mon
1-Tue
1-Wed
1-Thu
1-Fri
1-Sat
1-Sun

```



### 21 `while`/`do-while` Loops: Pure Statements 

`while` is a pure statement in Scala, While loops can’t return anything, they don’t work with `yield`.

In the below snippet, few things to notice - 

- usage of `var` to increment loop variable, mutable variables may have side-effects in code, problems
  in multithreaded applications etc
- The body of the `while` loop has to increment the loop variable
- The output can not be “composed” i.e. passed to a different function

```scala
scala> var x = 0
x: Int = 0

scala> while(x < daysOfWeek.size - 1) {
     |   val day = daysOfWeek(x)
     |   println(day)
     |   x += 1
     | }
Mon
Tue
Wed
Thu
Fri
Sat
```

While loops have a lot of clumsy syntax, hence, they are not used a whole lot in Scala

### Functions Vs Methods

Before going into this topic, we should first understand distinction between Functions and Methods in Scala.

> Functions are Objects, Methods are not
>
> Methods are associated with a class, functions are not

**Methods are not Objects**

The term `method`and `object` are often used interchangeably because methods can be stored in objects quite easily.

```scala
scala> def getArea (radius: Double): Double = {
     |   val PI =  3.14
     |   PI * radius * radius
     | }
getArea: (radius: Double)Double
```

**Functions are Objects**

Function objects are first class entities on par with Classes, methods are not

```scala
scala> val getArea = (radius: Double) => {
     |   val PI = 3.14
     |   PI * radius * radius
     | }: Double
getArea: Double => Double = <function1>

```

Functions and Methods - Differences

|                Functions                 |                 Methods                  |
| :--------------------------------------: | :--------------------------------------: |
| Functions are Value types - can be stored in val and var storage units | Methods are not Value types - cannot serve as r-values and are defined using def keyword |
| Functions are objects of type function0, function1....(traits descending from AnyRef) | Methods are not objects, but can be converted to function objects quite easily |
| Functions have both a type and a signature (tyoe is function0, function1 and so on) | Methods have signature, but no independent type |
|   Slightly slower and higher overhead    |  Slightly faster and better performing   |
| First class entities on par with classes | These are not first class entities unless converted to functions |
| Functions do not accept type parameters or parameter default values | Works fine with type parameters and parameter default values |



### 22 Functions are named, reusable expressions

In Scala, Functions are named, reusable expressions. 

- Like Expressions, **Functions** can be stored in values. variables and can be passed into other functions. This is because of Scala's support for **First Class Functions**. 
- Like Expressions, **Functions** have scopes and are influenced by variables from outside that scope. This is because of Scala's support for **Closures**

**Creating and Invoking a Function**

Creating a function is similar to creating an expression block, with simple changes to make it reusable and named. To create a function we need - 

- an expression or expression block
- a name for the expression or expression block
- Parameters that make the expression or expression block reusable
- Return type of the expression or expression block

In the snippet below,

- `getArea` is the name of the function, 
- `{length * breadth}` is the expression block that returns a value, 
- to make this expression block reusable, we specified parameters in `(length: Double, breadth: Double)` 
- `Double` specified after the expression block with a colon (:) is the return type of expression, we could even omit this return type and Scala would infer it via Type Inference.

```scala
scala> val getArea = (length: Double, breadth: Double) => {
     |   length * breadth
     | }: Double
getArea: (Double, Double) => Double = <function2>

// Invoking a function is intuitive
scala> getArea(5, 6)
res77: Double = 30.0

```



### 23 Assigning Methods to Values

In this section, we will see, how we can convert methods to functions. 

Let's start with a simple method 

```scala
scala> def getCircleArea(r: Double): Double = 3.14 * r * r
getCircleArea: (r: Double)Double
```

As a first step, try assigning above `method` to a `val`

```scala
scala> val computeArea = getCircleArea
<console>:8: error: missing arguments for method getCircleArea;
follow this method with `_' if you want to treat it as a partially applied function
       val computeArea = getCircleArea
                        ^

```

The above step errored out because, Scala is not sure whether you meant to:

- Invoke a method `getCircleArea` and store the result in  `computeArea`
- Or, Store the method `getCircleArea` itself in value `computeArea`

There are 2 ways to get around this - 

- Explicitly specifying that the signatures of `getCircleArea` and `computeArea` match
- Use a wildcard to specify that  `computeArea` has whatever signature `getCircleArea` has

**Explicitly specifying that the signatures of `getCircleArea` and `computeArea` match**:

**Signature of `getCircleArea` ?**

This method takes in a Double, and returns a Double. The signature of a method is simply the combination of its parameters and its return value. Methods have signatures, but not independent types.

In this method, Double goes in and Double comes out. 

> ​			(Double) => Double

Explicitly specifying the signature we can convert the method into a function and invoke it as below

```scala
scala> val computeArea: (Double) => Double = getCircleArea
computeArea: Double => Double = <function1>

scala> computeArea(10)
res78: Double = 314.0

```

**Using a WildCard :**

In the snippet specified in first step, the error gave us a hint, let us use it. This is known as **eta expansion**. ETA-expansion converts an expression of method type to an equivalent expression of function type.

```scala
scala> val computeAre = getCircleArea _
computeAre: Double => Double = <function1>

```

**Let’s do a couple more examples**

Example 1: 

```scala
// A simple method that takes in no parameters, and returns a double
scala> def getPI() = {PI}
getPI: ()Double

// Type of this method is () => Double

// Method 1:
scala> val calcPI: () => Double = getPI
calcPI: () => Double = <function0>

// Method 2:
scala> val calcPI = getPI _
calcPI: () => Double = <function0>

```

Example 2: 

```scala
// A simple method that takes in 2 parameters, and returns a double
scala> def getArea(l: Double, b: Double): Double = l * b
getArea: (l: Double, b: Double)Double

// Type of this method is (Double, Double) => Double

// Method 1:
scala> val calcArea: (Double, Double) => Double = getArea
calcArea: (Double, Double) => Double = <function2>

// Method 2:
scala> val calcArea = getArea _
calcArea: (Double, Double) => Double = <function2>

```



### 24 Invoking Functions with Tuples as Parameters

In this example, let's try invoking a function with an expression block returning a tuple.

Why? To be able to avoid breaking chains of function calls. This can only be done with functions, not methods. 

> ​			(getRectangleArea _).tupled()

Now, let’s say we had a square, whose perimeter we knew and we wanted to calculate the area of this
square, using the function `getArea`

```scala
scala> val perimeterOfSquare = 20.0
perimeterOfSquare: Double = 20.0

scala> // Step 1: Find the length of the side of the square

scala> val sideOfSquare = perimeterOfSquare/4
sideOfSquare: Double = 5.0

scala> // Step 2: call getArea with this length

scala> val area = getArea(sideOfSquare, sideOfSquare)
area: Double = 25.0

scala> // Combining both steps

scala> val area = getArea(perimeterOfSquare/4, perimeterOfSquare/4)
area: Double = 25.0

```

Scala has an even cooler way of doing this. Invoke the function using the result of this expression block.





```scala
scala> // Create an expression block that returns the length and breadth

scala> {
     |     val sideOfSquare = perimeterOfSquare/4;
     |     (sideOfSquare,sideOfSquare)
     | }
res81: (Double, Double) = (5.0,5.0)

scala> // Notice the result type is a tuple of two Doubles

scala> // Invoke the function using the result of this expression block

scala> (getArea _).tupled({
     |   val sideOfSquare = perimeterOfSquare/4
     |   (sideOfSquare,sideOfSquare)
     | })
res83: Double = 25.0

```

In the above snipped, the expression block returns a tuple.  `tupled` converts that tuple into a form that
a function can accept as parameters also called as **“Packing function parameters”**. `_` is used to convert `getArea` method into a function

**Why does this matter?**
Invoking Functions with Expression Blocks matters because this is yet another a way of chaining/composing functions, which is what functional programming is all about.

### 25 Named Method Parameters

While invoking a method, you can specify parameters by name. This way, the parameters need not be in the order in which they appear in the method definition.
Absolutely nothing changes while defining the method.

```
scala> def getArea(length:Double, breadth: Double) = {
     |   println(s"length - $length, breadth = $breadth")
     | }
getArea: (length: Double, breadth: Double)Unit

scala> getArea(breadth=5, length=10)
length - 10.0, breadth = 5.0

```

However, this works only with methods and not functions. It errors out as below

```scala
scala> val area = (length: Double, breadth: Double) => {
     |   println(s"length - $length, breadth = $breadth")
     |   length * breadth
     | }
area: (Double, Double) => Double = <function2>

scala> area(5,10)
length - 5.0, breadth = 10.0
res88: Double = 50.0

scala> area(breadth = 10, length = 5)
<console>:9: error: not found: value breadth
              area(breadth = 10, length = 5)
                   ^
```

**Why does this matter?**

Named parameters help a lot when calling method with default parameter values

### 26 Parameter Default Values

- A method (but not a function) can specify default values for any parameter.
- The method can then be invoked without specifying a value for that parameter
- Of course, the method can be invoked with that parameter too

```scala
scala> def getCircleStats(r: Double, PI: Double = 3.14) = {
     |   def getCircleArea(r: Double) = PI * r * r
     |   def getCircumference(r: Double) = 2 * PI * r
     |   (getCircleArea(r), getCircumference(r))
     | }
getCircleStats: (r: Double, PI: Double)(Double, Double)

scala> getCircleStats(4) // method invoked without specifying a value for parameter PI
res90: (Double, Double) = (50.24,25.12)

scala> getCircleStats(4, 3.1) // method can also be invoked by specifying a value for PI
res91: (Double, Double) = (49.6,24.8)

```

**Why does this matter?**

- Default parameters are a way to achieve code re-use. 


- In Scala any parameter can have a default value
- This is where the ability to specify parameters by name comes in handy

```scala
scala> def getCircleStats(PI: Double = 3.14, r: Double) = {
     |   def getCircleArea(r: Double) = PI * r * r
     |   def getCircumference(r: Double) = 2 * PI * r
     |   (getCircleArea(r), getCircumference(r))
     | }
getCircleStats: (PI: Double, r: Double)(Double, Double)

scala> getCircleStats(4) // Attempting to invoke the method the usual way leads to an error
<console>:11: error: not enough arguments for method getCircleStats: (PI: Double, r: Double)(Double, Double).
Unspecified value parameter r.
              getCircleStats(4)
                            ^

scala> getCircleStats(r = 4) // specifying the parameter by name works fine!
res93: (Double, Double) = (50.24,25.12)

```

Scala tries really hard to encourage code re-use by providing below language features - 

- Default Parameters
- Type Parameters
- Function Currying
- Partially Applied Functions

### 27 Type Parameters: Parametric Polymorphism

Note: This applies only to methods not to functions

Methods in Scala can be parameterized by type as well as value. The syntax is similar to that of generic classes. Type parameters are enclosed in square brackets, while value parameters are enclosed in parentheses.

Let’s check out an example of a method that takes in a key-value pair and prints the values and types of both items in the pair. Obviously, we need this method to work for all possible types of keys and values, example int, int or string, string and so on.
So - we specify 2 type parameters.

```scala
scala> def printPairTypes[K,V](k:K,v:V) = {
     |   val keyType = k.getClass
     |   val valueType = v.getClass
     |   println(s"$k, $v are of types $keyType,$valueType")
     | }
printPairTypes: [K, V](k: K, v: V)Unit

```

The type parameters are in square brackets as part of the method definition. K is the type of the key, V is the type of the value. The method parameters now are expressed in terms of the type parameters k, v.

```scala
scala> printPairTypes(12,"12"); 
12, 12 are of types class java.lang.Integer,class java.lang.String

scala> printPairTypes(12,'a');
12, a are of types class java.lang.Integer,class java.lang.Character

```

**Type Parameters work only with Methods, Not Functions**

Reason: When we convert method to a function as below, we lose type parameter info.

Using the placeholder _ causes type parameters to be converted to Any (i.e. lost)

```scala
scala> val fnPrintPairTypes = printPairTypes _
fnPrintPairTypes: (Any, Any) => Unit = <function2>

```

To overcome this, we need to explicitly specify the type parameter values for each function object to be properly specified

```scala
scala> val fnPrintPairTypes = printPairTypes[Int, String] _
fnPrintPairTypes: (Int, String) => Unit = <function2>

```

### 28 Vararg Parameters


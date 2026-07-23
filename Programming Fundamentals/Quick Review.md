# Table of Content

### Core Topic

[Variables](#variables)
1. [Variables](#variables)

[Data Types](#data-types)
1.   [Primitive Data Types](#1-primitive-basic-data-types)
2.   [Non-Primitive Data Types](#2-non-primitive-data-types)
3.   [Numeric Types](#3-numeric-types)
4.   [Boolean Type](#4-boolean-type)
5.   [Character & String](#5-character--string)
6.   [Static vs Dynamic Typing](#6-static-vs-dynamic-typing)
7.   [Strong vs Weak Typing]()
8.   [Type Inference]()
9.   [Type Conversion]()
10.   [Null / None / Nil]()

[Functions]()

[Scope]()

[Recursion]()

[Arrays]()

[Strings]()

[Pointers / References]()

[Memory Management]()

[Object-Oriented Programming]()

[Interfaces]()

[Generic Programming]()

[Lambda / Delegates (language dependent)]()

[Exception Handling]()

[Const Correctness]()

[Static vs Dynamic Allocation]()

[Resource Lifetime]()


⏬ [To bottom](#-bottom-link-anchor)
***

# Variables


## 1. Variables
### One Sentence Definition

A **variable** is a named storage location that holds a value, allowing a program to store, retrieve, and modify data during execution.

### Why Do We Need It?

Variables allow data to be stored, reused, updated, and shared between different parts of a program instead of hardcoding values everywhere.

It's the core component making program capable of handling changing data.

### Core Idea

A variable consists of three essential parts:

-   **Name (Identifier):** How the program refers to the stored data.
-   **Type (in statically typed languages):** Defines what kind of value can be stored.
-   **Value:** The actual data currently stored.

"A container with name tag, and a restriction declare what can be store in it."

### Key Characteristics

-   Has a unique identifier (name).
-   Stores a value that may change over time.
-   Has a data type (explicit or inferred in many languages).
-   Exists only within a certain scope and lifetime.
-   Can usually be read and written multiple times unless declared as immutable or constant.

### Advantages

N/A

### Disadvantages

N/A

### Common Use Cases

Every where in programming realm. No variable mean no way of constructure a dynamic program, it's madatory for input handling, calculation, confuguration, counter and even more.

### Comparison

| Concept | Purpose |
| --- | --- |
| Variable | Stores data that can usually change. |
| Constant | Stores data that should not change after initialization. |
| Literal | A fixed value written directly in code (e.g., `10`, `"Hello"`). |
| Expression | Produces a value, often using variables and operators. |

### Things People Often Confuse

N/A

### Things You MUST Remember

-   Every variable has a scope and lifetime, even if you don't explicitly see them.
-   A variable's value may change, but its identity (its name) remains the same.

***

# Data Types

##### What is a Data Type?

The foundation of the chapter.

Covers:

-   Definition of a data type
-   Why variables need types
-   How types determine what values and operations are allowed

## 1. Primitive (Basic) Data Types

### One Sentence Definition

**Primitive data types** are the most basic, built-in data types provided by a programming language that store a single, simple value.

### Why Do We Need It?

Computers process different kinds of information—numbers, text, and logical values. Primitive data types define the fundamental categories of data, allowing the compiler or interpreter to know how to store, interpret, and operate on each value efficiently.

Without primitive data types, a programming language would have no standardized way to represent basic information.

### Core Idea

Primitive data types are the **building blocks** of all other data types. They represent a single piece of data and are directly supported by the language and hardware.

Most complex data structures (such as arrays, classes, or objects) are ultimately built using primitive data types.

Common primitive data types include:

-   **Integer** – Whole numbers
-   **Floating-point** – Decimal numbers
-   **Boolean** – `true` or `false`
-   **Character** – A single text character

> **Note:** The exact set of primitive data types varies by programming language. For example, some languages treat `String` as a primitive type, while others treat it as an object.

### Key Characteristics

-   Built into the programming language.
-   Store a **single** value.
-   Usually have a fixed size and range.
-   Optimized for speed and memory efficiency.
-   Serve as the foundation for more complex data types.

### Advantages

-   Fast to read and write.
-   Efficient memory usage.
-   Directly supported by the language and CPU.

### Disadvantages

-   Can only represent simple values.
-   Limited by their predefined size and range (e.g., integer overflow).

### Common Use Cases

-   **Integer** – Counting items, indexing arrays, loop counters.
-   **Floating-point** – Measurements, scientific calculations, percentages.
-   **Boolean** – Conditions, flags, decision making.
-   **Character** – Processing individual letters or symbols.

### Comparison

| Primitive Data Types | Non-Primitive Data Types |
| --- | --- |
| Built into the language | Built using primitive types (or language features) |
| Store a single simple value | Can store multiple values or behaviors |
| Generally fixed in size | Often variable or user-defined |
| Simple and lightweight | More flexible and expressive |

### Things People Often Confuse

##### *Character vs String*

A **character** represents a single symbol.

```
'A'
```

A **string** represents a sequence of characters.

```
"Apple"
```

Not every language considers `String` a primitive type.

### Things You MUST Remember

-   Primitive data types are the **fundamental building blocks** of a programming language.
-   They represent **one simple value**.
-   The exact primitive types depend on the programming language.
-   Primitive types are designed for **speed, simplicity, and efficiency**.
-   Complex data structures are generally built upon primitive data types.

## 2. Non-Primitive Data Types

### One Sentence Definition

**Non-primitive data types** are data types that are built from primitive data types or provided by the language to represent more complex data, relationships, or behaviors.

### Why Do We Need It?

Real-world applications often need to represent collections of data, objects with properties, or entities with both data and behavior. Non-primitive data types make it possible to model these more complex structures.

Without non-primitive data types, building applications such as games, web applications, or databases would be extremely difficult and repetitive.

### Core Idea

Non-primitive data types allow multiple pieces of data—or even functions and behaviors—to be grouped into a single entity. They provide higher-level abstractions that make programs easier to organize, maintain, and extend.

Some common examples include:

-   **String** – A sequence of characters.
-   **Array** – An ordered collection of elements.
-   **Object/Class** – A collection of data (and often behavior) representing a real-world entity.
-   **List, Map, Set** – Specialized collections for storing and organizing multiple values.

> **Note:** The exact definition of a non-primitive type varies by language. For example, `String` is considered a primitive type in some languages but an object or reference type in others.

### Key Characteristics

-   Can store multiple values or represent complex data.
-   Often built using primitive data types.
-   May include both data and behavior (e.g., objects).
-   Generally more flexible than primitive types.
-   Usually support methods or operations beyond simple arithmetic.

### Advantages

-   Can model real-world entities and relationships.
-   Organize related data into meaningful structures.
-   Improve code readability and maintainability.
-   Enable code reuse through reusable data structures and objects.
-   Support more advanced programming techniques, such as object-oriented programming.

### Disadvantages

-   Generally require more memory than primitive types.
-   May have additional performance overhead.
-   Behavior and implementation can vary significantly between programming languages.

### Common Use Cases

-   **String** – Storing names, messages, or text.
-   **Array/List** – Storing collections of values.
-   **Object/Class** – Representing users, products, vehicles, or game characters.
-   **Map/Dictionary** – Associating keys with values.
-   **Set** – Storing unique elements.

### Comparison

[**Check primitive data types**](#comparison-1)

### Things People Often Confuse

##### *Non-Primitive vs Data Structure*

Not every non-primitive type is a **data structure**.

For example:

-   `String` → Non-primitive type, but not usually considered a data structure in CS.
-   `Array`, `List`, `Map` → Both non-primitive types **and** data structures.

A data structure focuses on **how data is organized**, while a non-primitive type is a broader programming concept.

### Things You MUST Remember

-   Non-primitive data types exist to represent **more complex information** than primitive types can.
-   They often contain **multiple values**, **relationships**, or **behavior**.
-   The exact set of non-primitive types differs between programming languages.

## 3. Numeric Types

### One Sentence Definition

**Numeric types** are data types used to represent numerical values for arithmetic operations, calculations, and measurements.

### Why Do We Need It?

Not all numbers are the same. Some numbers represent whole quantities (e.g., the number of users), while others represent values with fractional parts (e.g., temperature or distance). Different numeric types allow programs to balance **precision**, **range**, and **memory usage** based on the problem being solved.

### Core Idea

Numeric types can be broadly divided into two categories:

-   **Integer Types (int)** – Represent whole numbers without a fractional part.
-   **Floating-Point Types (float)** – Represent numbers with decimal or fractional values.

Different numeric types have different characteristics, including:

-   **Range** – The minimum and maximum values they can store.
-   **Precision** – How accurately they can represent values.
-   **Memory Size** – The amount of memory required to store the value.

Choosing the appropriate numeric type helps prevent errors such as overflow, underflow, or precision loss.

### Key Characteristics

-   Represent numerical values.
-   Support arithmetic operations such as addition, subtraction, multiplication, and division.
-   Have a limited range of representable values.
-   May trade precision for a larger range or better performance.

### Advantages

-   Efficient storage and computation for numerical data.
-   Provide specialized types for different mathematical needs.
-   Directly supported by computer hardware and programming languages.

### Disadvantages

-   Floating-point types may introduce rounding errors.
-   Choosing the wrong numeric type can lead to incorrect calculations or wasted memory.
-   Behavior (size and precision) may differ between programming languages and platforms.

### Common Use Cases

| Numeric Type | Common Uses |
| --- | --- |
| Integer | Counting, indexing, IDs, loop counters |
| Floating-point | Measurements, physics simulations, financial approximations*, graphics calculations |

> **Note:** Financial applications often avoid floating-point numbers because small rounding errors can accumulate. Many systems use fixed-point or decimal types instead.

### Comparison

| Integer | Floating-Point |
| --- | --- |
| Exact representation | Approximate representation |
| No decimal point | Supports decimal values |

### Things People Often Confuse
##### *Precision vs Accuracy*

These terms are related but not identical.

-   **Precision** refers to how many digits a type can reliably represent.
-   **Accuracy** refers to how close a value is to the true or expected value.

A floating-point number can have high precision yet still be slightly inaccurate due to how it is stored internally.

##### *Range vs Precision*

A larger **range** means the type can represent much larger (or smaller) numbers.

Higher **precision** means the type can represent values with greater exactness.

Increasing one often requires sacrificing the other or using more memory.

### Things You MUST Remember

-   Numeric types are primarily divided into **integers** and **floating-point numbers**.
-   Integers are **exact** but cannot represent fractions.
-   Floating-point numbers can represent fractions but are **approximations**.
-   Every numeric type has a limited **range** and **precision**.
-   Choose the numeric type based on the requirements of the problem, not simply because it "works."
-   Never compare floating-point values for exact equality unless you understand the implications; use a tolerance (epsilon) when appropriate.

## 4. Boolean Type

### One Sentence Definition

The **Boolean type** is a data type that represents one of two logical values: **`true`** or **`false`**.

### Why Do We Need It?

Programs constantly make decisions:  Boolean type provides a simple and standardized way to represent these **yes/no**, **on/off**, or **true/false** conditions.

Without Booleans, programs would have to rely on arbitrary values (such as `0` and `1`) to represent logical states, making code **less readable** and more **error-prone**.

### Core Idea

A Boolean value answers a question with only two possible outcomes:

-   **`true`** – The condition is satisfied.
-   **`false`** – The condition is not satisfied.

Booleans are typically produced by:

-   Comparison operations (`==`, `>`, `<`, etc.)
-   Logical operations (`AND`, `OR`, `NOT`)
-   Functions that return success/failure or yes/no results

### Key Characteristics

-   Has only two possible values: `true` and `false`.
-   Usually occupies very little memory (implementation varies by language).
-   
### Advantages

-   Makes program logic clear and easy to understand.
-   Improves code readability compared to using numeric flags.

### Disadvantages
N/A

### Common Use Cases

-   Checking conditions in `if` statements.
-   Control signal loops (`while`, `for`).
-   Indicating success or failure of an operation.
-   Tracking program states (e.g., `isRunning`, `isVisible`, `hasPermission`).

### Comparison
N/A

### Things People Often Confuse

##### *Boolean vs Bit*

A **Boolean** is a programming language concept representing a logical value.

A **bit** is the smallest unit of data in computer hardware.

Although a Boolean may be stored using one bit (or more, depending on the language and hardware), the two concepts are not the same.

##### *Boolean vs Truthy/Falsy Values*

Many languages (such as Python and JavaScript) allow non-Boolean values to be treated as `true` or `false`.

For example:

```
0        → false
1        → true
""       → false
"Hello"  → true
```

However, these values are **not** Booleans—they are values that can be **implicitly converted** to a Boolean.

Languages like Java and C# generally require an actual Boolean value in conditional statements.

### Things You MUST Remember

-   A Boolean can only be **`true`** or **`false`**.
-   Booleans are used for **decision-making**, not calculations.
-   Comparison operations produce Boolean values.
-   Logical operators work on Boolean values.
-   Be aware that some languages support **truthy/falsy** conversions while others require explicit Boolean values.

## 5. Character & String

### One Sentence Definition

A **character** represents a single text symbol, while a **string** represents an ordered sequence of one or more characters used to store and manipulate text.

### Why Do We Need It?

 Character and string types provide a standardized way to represent and manipulate textual information.

Without them, handling human-readable data would be extremely difficult.

### Core Idea

Although both deal with text, **characters** and **strings** serve different purposes.

-   A **character** stores **one** text symbol.
-   A **string** stores **multiple** characters in sequence.

A string can be thought of as a collection of characters arranged in a specific order.

Most programming languages provide many built-in operations for strings, such as searching, concatenation, comparison, and extracting substrings.

> **Note:** While a string is conceptually a sequence of characters, how it is implemented varies by language. Some languages treat strings as arrays of characters, while others implement them as specialized objects.

### Key Characteristics

#### Character

-   Represents a single symbol.
-   Typically enclosed in **single quotes** (`'A'`) in many languages.
-   Can represent letters, digits, punctuation, or special symbols.
-   Often has a fixed size.

#### String

-   Represents a sequence of characters.
-   Typically enclosed in **double quotes** (`"Hello"`).
-   Can be empty (`""`).

### Advantages

#### Character

-   Efficient for storing individual symbols.
-   Useful when processing text one character at a time.

#### String

-   Easy to store and manipulate text.
-   Rich set of built-in operations.
-   Essential for user interaction and file processing.

### Disadvantages

#### String

-   String operations can become expensive for very large texts.
-   Some languages use immutable strings, meaning modifications create new string objects.

### Common Use Cases

#### Character

-   Reading keyboard input one key at a time.
-   Processing individual letters.
-   Checking whether a character is a digit, letter, or punctuation.

#### String

There's way to many use case for string, just name a few.

-   Usernames and passwords.
-   Messages and documents.
-   File paths and URLs.
-   JSON, XML, and source code.
-   Displaying information to users.

### Comparison

[Check Key Characteristics](#key-characteristics-5)

### Things People Often Confuse

##### *Character vs String*

These are **not interchangeable** most of the time.

##### *String vs Character Array*

Implementation differs by language:

-   In **C**, a string is an array of characters ending with a null terminator (`'\0'`).
-   In **Java**, **C#**, and **Python**, a string is a dedicated type with built-in methods.

As a programmer, it's more important to understand that a string **behaves like text**, regardless of its internal implementation.

##### *String Length vs Memory Size*

A string's **length** is the number of characters it contains.

Its **memory usage** depends on:

-   Character encoding (ASCII, UTF-8, UTF-16, etc.)
-   Language implementation
-   Internal metadata

A string with five characters does **not** necessarily occupy five bytes.

##### *String Is (Usually) Not a Primitive Type*
In real world example:

-   Java → Object
-   C# → Reference type (`System.String`)
-   Python → Object
-   JavaScript → Primitive value (with object-like behavior)
-   C → Character array

### Things You MUST Remember

-   A **character** represents **one** symbol.
-   A **string** represents a **sequence of characters**.
-   `"A"` and `'A'` are often different data types.
-   Strings provide many built-in operations for processing text.
-   The implementation of strings differs between programming languages, but the concept remains the same.

## 6. Static vs Dynamic Typing

### One Sentence Definition

**Static typing** checks a variable's type before the program runs, while **dynamic typing** determines a variable's type during program execution.

### Why Do We Need It?

Programming languages need a way to determine what kind of data a variable holds and whether operations on that data are valid. Static and dynamic typing are two different approaches to enforcing type rules, each balancing **safety**, **flexibility**, and **development speed**.

### Core Idea

The key difference is **when type checking occurs**.

#### Static Typing

The compiler verifies that variables are used with the correct data types **before** the program executes.

```
Compilation → Type Checking → Program Runs
```

Errors such as assigning a string to an integer variable are usually caught during compilation.

Examples:

-   C
-   C++
-   C#
-   Java
-   Go
-   Rust

#### Dynamic Typing

The type of a variable is determined and checked **while the program is running**.

```
Program Runs → Type Checking Happens During Execution
```

Variables can often hold different types of values throughout their lifetime.

Examples:

-   Python
-   JavaScript
-   Ruby
-   PHP

### Key Characteristics

#### Static Typing

-   Type checking occurs before execution.
-   Variables usually have a fixed type.
-   Many type-related errors are detected early.
-   Often provides better IDE support and compile-time optimization.

#### Dynamic Typing

-   Type checking occurs during execution.
-   Variables can often reference different data types over time.
-   More flexible for rapid development.
-   Type-related errors may only appear when the affected code is executed.

### Advantages

#### Static Typing

-   Detects many bugs before runtime.
-   Better autocomplete and refactoring support.
-   Easier to maintain large codebases.
-   Can improve runtime performance through compiler optimizations.

#### Dynamic Typing

-   Less code to write.
-   Faster prototyping.
-   Convenient for scripting and automation.

### Disadvantages

#### Static Typing

-   More verbose in some languages.
-   Requires defining or inferring types before use.

#### Dynamic Typing

-   More runtime type errors.
-   Harder to catch bugs before deployment.
-   Can become difficult to maintain in very large projects.
-   IDEs may have less information for static analysis.

### Common Use Cases

#### Static Typing

-   Enterprise software
-   Large-scale systems
-   Financial systems
-   Operating systems
-   Performance-critical applications

#### Dynamic Typing

-   Scripts and automation
-   Web development
-   Rapid prototyping
-   Small to medium-sized applications
-   Data analysis (e.g., Python)

### Comparison

| Static Typing | Dynamic Typing |
| --- | --- |
| Type checked before execution | Type checked during execution |
| Errors found earlier | Errors may appear at runtime |
| Usually fixed variable types | Variables can often change types |
| Better compiler optimization | Greater flexibility |
| Preferred for large projects | Preferred for rapid development |

### Things People Often Confuse

##### _Static Typing vs Type Inference_

These are **different concepts**.

Static typing describes **when** types are checked.

Type inference describes **whether the programmer must explicitly write the type**.

For example:

```
var age = 20;
```

Although the type isn't written, `age` is still inferred as an `int` and remains **statically typed**.

Many people mistakenly think `var` automatically means dynamic typing.

##### _Dynamic Typing vs Weak Typing_

These terms are unrelated.

-   **Dynamic typing** answers **when** type checking happens.
-   **Weak typing** describes **how strictly** the language enforces type rules.

A language can be:

-   Statically typed and strongly typed (e.g., C#, Java)
-   Dynamically typed and strongly typed (e.g., Python)
-   Dynamically typed and weakly typed (e.g., JavaScript)

### Things You MUST Remember

-   **Static typing** performs type checking **before** program execution.
-   **Dynamic typing** performs type checking **during** program execution.
-   Static typing generally catches errors earlier, while dynamic typing offers greater flexibility.
-   **Type inference is not the same as dynamic typing.**
-   **Dynamic typing is not the same as weak typing.**
-   Neither approach is universally better—the choice depends on the language's goals and the application's requirements.

***

> [!INFO]   Editing tool
> #####  ⚓ Bottom Link Anchor
> ⏫ [To top](#table-of-content)
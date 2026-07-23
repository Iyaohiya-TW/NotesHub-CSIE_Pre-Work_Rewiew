# Table of Content

### Core Topic

[Variables](#variables)
1. [Variables](#variables)

[Data Types](#data-types)
1.   [Primitive Data Types](#1-primitive-basic-data-types)
2.   [Non-Primitive Data Types](#2-non-primitive-data-types)
3.   [Numeric Types](#3-numeric-types)
4.   [Boolean Type]()
5.   [Character & String]()
6.   [Static vs Dynamic Typing]()
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


⏬ [To bottom](#bottom-link-anchor)
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

### One-Minute Summary

N/A

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

#### Character vs String

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

### One-Minute Summary

Primitive data types are the simplest built-in types provided by a programming language. They store a single value, such as an integer, decimal number, Boolean value, or character. Because they are directly supported by the language and hardware, they are fast, memory-efficient, and form the foundation for all more complex data types. Although different programming languages define primitive types differently, the underlying concept remains the same: they are the basic units used to represent data in a program.

***

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

##### Non-Primitive vs Data Structure

Not every non-primitive type is a **data structure**.

For example:

-   `String` → Non-primitive type, but not usually considered a data structure in CS.
-   `Array`, `List`, `Map` → Both non-primitive types **and** data structures.

A data structure focuses on **how data is organized**, while a non-primitive type is a broader programming concept.

### Things You MUST Remember

-   Non-primitive data types exist to represent **more complex information** than primitive types can.
-   They often contain **multiple values**, **relationships**, or **behavior**.
-   The exact set of non-primitive types differs between programming languages.

### One-Minute Summary

Non-primitive data types are higher-level types used to represent complex data that cannot be expressed by a single primitive value. Examples include strings, arrays, objects, lists, maps, and sets. They often combine multiple primitive values into meaningful structures and may also include behavior through methods. While they require more memory and are generally more complex than primitive types, they make it possible to model real-world problems effectively and form the foundation of modern software development.

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

***

> [!INFO]   Editing tool
  > #####  ⚓Bottom Link Anchor
> ⏫ [To top](#table-of-content)
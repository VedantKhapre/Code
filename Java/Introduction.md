# Java Data Types

## Theory
Java is a strongly-typed language, which means every variable must have a declared type. Data types in Java are divided into two categories:

### Primitive Data Types
- Store simple values
- Stored directly in memory (stack)
- Have fixed size
- Eight types: byte, short, int, long, float, double, char, boolean
- Cannot be null
- Start with lowercase letters

### Reference Data Types (Objects)
- Store complex objects
- Stored in heap memory (reference stored in stack)
- Variable size
- Examples: String, Arrays, Classes
- Can be null
- Start with uppercase letters

## Memory Allocation
```
Stack Memory                  Heap Memory
+-------------+              +----------------+
| int x = 5   |              | String str     |
| boolean y   |              | Objects        |
| References  |------------->| Arrays         |
+-------------+              +----------------+
```

## Numerical Types

### Mainly Used
```java
int aNumber = 42;                    // Integer (or Whole Number) [-2,147,483,648 to 2,147,483,647]
float aFloatingNumber = 13.37f;      // Floating point number  [7 decimal point precision]
double aDoubleNumber = 420.0005;     // Double number  [15 decimal point precision]
```

### Sometimes Used
```java
byte aTinyNumber = 100;              // One byte (or 8 bits) stores numbers from [-128 to 127]
short aSmallNumber = 30000;          // short stores numbers from [-32,768 to 32,767]
long aLongNumber = 50000000L;        // Long (for really long numbers) [-9,223,372,036,854,775,808 to 9,223,372,036,854,775,807]
```

## Logic Types
```java
boolean isThisJAVA = true;          // Store either true (1) or false (0)
boolean isThisHTML = false;
```

## Text Types
```java
char aSingleCharacter = 'j';         // Stores a single Character. Can also include special Characters like commas, dashes etc.
String message = "Hello World";      // Store a sequence of characters.
String test = null;                  // null is not 0, but literally empty. Has no value!
```

## Type Conversion
### Implicit Conversion (Widening)
```java
int myInt = 100;
double myDouble = myInt;    // Automatic conversion from int to double
```

### Explicit Conversion (Narrowing)
```java
double myDouble = 9.78;
int myInt = (int) myDouble;    // Manual conversion, decimal part is truncated
```

## Common Use Cases
- `int`: Counting, array indices, simple calculations
- `double`: Scientific calculations, precise decimal values
- `boolean`: Flags, condition checking
- `String`: Text processing, user input
- `long`: Time in milliseconds, very large numbers
- `float`: When memory is constrained and full precision isn't needed

## Important Notes
Remember to add:
- 'f' suffix for float values
- 'L' suffix for long values

## Memory Size Reference
- byte: 8 bits
- short: 16 bits
- int: 32 bits
- long: 64 bits
- float: 32 bits
- double: 64 bits
- char: 16 bits
- boolean: 1 bit
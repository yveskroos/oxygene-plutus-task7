# Haskell Type Classes and Custom Types Exercises

## Table of Contents

1. [Eq Instance for Color](#eq-instance-for-color)
2. [Ord Instance for Color](#ord-instance-for-color)
3. [Function with Multiple Constraints](#function-with-multiple-constraints)
4. [Show and Read for Shape](#show-and-read-for-shape)
5. [Numeric Function](#numeric-function)
6. [Integral and Floating](#integral-and-floating)
7. [Bounded and Enum](#bounded-and-enum)
8. [String Parsing](#string-parsing)
9. [Custom Type Class](#custom-type-class)
10. [Multiple Constraints Function](#multiple-constraints-function)

## Eq Instance for Color

Implements the `Eq` type class for a custom `Color` data type (with constructors Red, Green, Blue). Two colors are considered equal if they are the same constructor.

## Ord Instance for Color

Implements the `Ord` type class for the `Color` type, establishing the ordering Red < Green < Blue. This allows colors to be compared and sorted.

## Function with Multiple Constraints

Implements a generic `compareValues` function that takes two values of any type that implements both `Eq` and `Ord` type classes, and returns the larger value.

## Show and Read for Shape

Defines a `Shape` algebraic data type with `Circle` and `Rectangle` constructors, and implements `Show` and `Read` instances for proper string representation and parsing.

## Numeric Function

Implements a `squareArea` function that calculates the area of a square given its side length, working with any numeric type that implements the `Num` type class.

## Integral and Floating

Defines a `circleCircumference` function that calculates a circle's circumference (2πr) and works with both integral and floating-point numbers through appropriate type class constraints.

## Bounded and Enum

Implements a `nextColor` function that cycles through the `Color` values in order (Red → Green → Blue → Red), utilizing `Bounded` and `Enum` instances for the type.

## String Parsing

Creates a `parseShape` function that attempts to read a `Shape` from a string input, returning `Nothing` for invalid inputs, demonstrating safe parsing with the `Read` type class.

## Custom Type Class

Defines a `Describable` type class with a `describe` method, and implements instances for both `Bool` and `Shape` types to provide descriptive text for each.

## Multiple Constraints Function

Implements a `describeAndCompare` function that works with any two values of types implementing both `Describable` and `Ord` type classes, returning the description of the larger value.

## Usage

These exercises demonstrate practical uses of Haskell's type class system. To use them:
1. Load the module in GHCi
2. Create values of the custom types
3. Call the implemented functions

## Requirements
- GHC (Glasgow Haskell Compiler)
- Understanding of Haskell's type system and type classes

## License
This code is provided for educational purposes. Free to use and modify.

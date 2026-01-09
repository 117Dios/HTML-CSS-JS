# Operator: `typeof`

`typeof` is unary (takes only one argument) and returns a string that tells the data type of the given argument.

Example:

```javascript
let  year  =  1990;
console.log(typeof  year);  //  ->  number
console.log(typeof  1991);  //  ->  number
   
let  name  =  "Alice";
console.log(typeof  name);  //  ->  string
console.log(typeof  "Bob");  //  ->  string
   
let  typeOfYear  =  typeof  year;
console.log(typeOfYear);  //  ->  number
console.log(typeof  typeOfYear);  //  ->  string
```

<hr><hr>

# Primitive data types

## Boolean

Can be `true` or `false`. Can be used as a flag to check for something. The variable name is usually preceded by "is" when used like this.

## Number

Represents both integers and real numbers. For correctness of calculations, integer values should be limited to the range of [-(2<sup>53</sup>-1), (2<sup>53</sup>-1)]

A number can also be represented in forms other than decimals, if using the appropriate prefix:

- `0x...`: hexadecimal
- `0o...`: octal
- `0b...`: binary

We can also write exponential numbers:

- 9000 &rarr; `9e3`
- 0.00123 &rarr; `123e-5`

There are also `Infinity`, `-Infinity` and `NaN` for "Not a Number" (Type of error)

## BigInt

Not used often, but allows to use integers of virtually any length. Can be used for all the operations of a normal integer, but during the division the result will **always** be rounded down to the nearest integer.

BigInt variables can only be used with other BigInts in operations. Using a Number will result in a TypeError.

BigInt does not have an equivalent of `Infinity`, `-Infinity`and `NaN`. Instead, there will be an error.

BigInts are defined with the `n` suffix:

```javascript
let  big  =  1234567890000000000000n;
let  big2  =  1n;
   
console.log(big);  //  ->  1234567890000000000000n
console.log(typeof  big);  //  ->  bigint
   
console.log(big2);  //  ->  1n
console.log(7n  /  4n);  //  ->  1n
```

# String


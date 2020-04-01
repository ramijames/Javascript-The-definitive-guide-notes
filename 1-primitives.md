Javascript: https://raw.githubusercontent.com/ramijames/Javascript-The-definitive-guide-notes/master/javascript-the-definitive-guide.png

# Javascript Basics

This is part of an on-going series where I reinterpret [“Javascript: The definitive guide”](https://amzn.to/34916jT) into the core concepts as I relearn them. Consider this my cliff notes. I hope helps someone else learn the ins and outs of the language.
Types, Values, and Variables

Javascript types can be divided into two categories: primitive types (which you inherit from) and object types (which is most of what JS is).

## The basic primitive types are

| Primitives | Example    |
| ----------:|-----------:|
| Numbers    | 123        |
| Strings    | "Hello"    |
| Booleans   | True/False |

You also have special primitive types like null and undefined. Anything besides these five primitives is an object.

There is one very special object, the global object, which everything is inherited from.

## About Objects

Basic JavaScript objects are unordered collections of named values. They look like this:

```javascript
{
    “key” : “value”,
    “key” : “value”
}
```

Each object is comprised of sets of primitive objects. Objects can contain other objects and be nested to create deeply complex objects.

```javascript
{
    “booktitle” : “Javascript: The Definitive Guide”,
    details: {
        “author” : ”David Flanagan“,
        “ISBN” : 978-1491952023 
    }
}
```

Arrays are a special kind of object which uses the bracket [ ] notation. It is an ordered collection of values.

## About Numbers

JavaScript is different than languages like C++ where there are different types of numbers which use different amounts of memory. What you lose in control, you gain in flexibility.

In addition to the regular base-10 integers we are used to using in day to day life, JavaScript supports hexadecimal numbers (base-16). They start with Ox followed by a string of numbers and letters. A hexadecimal number is represented by 0 through 9 and the letters A through F, which represent 10- 16.

So in Hexadecimal, Oxff is 15 *16 + 15, which gives us 255 in base-10.

## Math in JavaScript

There are all the basic operators which you are familiar with like + , -, /,* etc. Core JavaScript also provides you with a series of Math functions for complex mathematics.

```javascript
Math.pow(2,53)              //=> 9007199254740992: 2 to the power of 53
Math.round(0.6)             //=> 1.0: round up
Math.ceil(0.6)              //=> 1.0: round up
Math.floor(0.6)             //=> 0.0: round down
Math.abs(-5)                //=> 5: return the absolute number
Math.max(x,y,z)             //=> Return the largest argument
Math.min(x,y,z)             //=> Return the smallest argument
Math.random                 //=> Returns a pseudo-random number
Math.PI                     //=> Returns PI
Math.E                      //=> Returns e, the base of the natural log
Math.sqrt(3)                //=> The square-root of 3
Math.pow(3, 1/3)            //=> The cube of 3
Math.sin(0)                 //=> Trigonomotry, also Math.cos, Math.atan, etc.
Math.log(10)                //=> Natural log of ten
Math.log(100)/Math.LN10     //=> Base 10 log of 100
Math.log(512)/Math.LN2      //=> Base 2, log of 512
Math.exp(3)                 //=> Math.E cubed
 
```

## Dates and Times 

The last topic we’ll cover is how core JavaScript includes a Date() constructor for creating objects that represent time.

```javascript

var time = new Date(2010,0,1)

time.getFullYear()          // 2020
time.getMonth()             // 0 (January)
time.getDay()               // 1

```
And that takes us through the first 40 or so pages of the book, up to dealing with String Literals, the next article that I’ll publish.
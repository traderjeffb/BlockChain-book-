# Solidity value types

* bool
* uint
* int
* address
* string
* enum 

Above is a list of the most common value type variables. \(for a complete list see the Solidity documentation\) These types_ "are called value types because variables of these types will always be passed by value, i.e. they are always copied when they are used as function arguments or in assignments." _

_source: _[http://solidity.readthedocs.io/en/v0.4.21/types.html?highlight=value types](http://solidity.readthedocs.io/en/v0.4.21/types.html?highlight=value types)

### What is the difference between reference types and value type of variables?

When we call functions, as we did in the "Intro to Remix" section,  any value type of variable received a copy of the variable when it as called. If the variable were a reference type you would only get the address of the variable but not a copy. The difference will become much clearer with a few examples. Keep in mind that when programming in Solidity you can't assign variable outside of functions. You have to create constructors which we will discuss later. 


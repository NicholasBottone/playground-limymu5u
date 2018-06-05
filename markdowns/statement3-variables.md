# Variables

You may recall on the last activity we briefly mentioned **variables**.  We're going to take an in depth look at variables right now.

## What is a variable?

A **variable** is a value that can change, depending on conditions or on information passed to the program. Typically, a program consists of instructions that tell the computer what to do and data that the program uses when it is running.

You can think of a variable as a container or bin that can hold hold little pieces of information and data.  A variable could hold a **number**, a **letter*, a **word**, or a **sentence**.

## Types of Primative Variables

There are eight primative types of variables used in Java, each of which serving distinct purposes.

### boolean

The simplest, most basic type of variable is called a `boolean`.  The boolean variable can only have two states: `true` or `false`.  

The boolean variable is **binary** -- that is, it only has two states.  It is either **on** or it is **off**.  It is either **1** or it is **0**.  `true` or `false`.

```java runnable
// { autofold
public class Main {
  public static void main(String args) {
  // }
  boolean a = false;
  boolean b = true;
  
  System.out.println(a);
  System.out.println(b);
// { autofold
  }
}
// }
```

You can declare a boolean variable by typing the word "boolean" followed by a space and then the name of the variable to be created.  
For example, to create a boolean called `isAwesome`, just type `boolean isAwesome;`.  Don't forget to end the line with a semicolon!

You can assign a value to a boolean by using the equals sign. `=`  
For example, to set the `isAwesome` variable to `true` after it has already been created, just type `isAwesome = true;`.  
To declare and assign a value to a variable on the same step, you can use `boolean isAwesome = true`.  This is the same procedure shown above with the `a` and `b` booleans.

Try pressing the run code button.  The two booleans `a` and `b` will be printed to the console.  Try creating more boolean variables and printing them to the console above.  Try switching the order of the values.  See how it affects the output.

### Numerals

Numbers are slightly more complex to store in variables, since there are several different types of numbers.  Some numbers have decimals after them, some numbers are negative, and some numbers are just massive.  There are several different types of variables in Java to handle some of these situations.

#### int

The most basic numeral variable is an integer (`int`).  An `int` variable can be positive or negative, as long as it is a whole number and has no decimal places.  There is technincally a limit to the size of the number that an integer variable can hold, but it is so massive that you don't normally have to worry about it.  The integer variable can hold numbers from -2^31 to 2^31 - 1 (-2,147,483,648 to 2,147,483,647).

```java runnable
// autofold {
public class Main {
  public static void main(String[] args) {
    // }
    int num1 = 3;
    int num2 = 6;
    int sum = num1 + num2;
    
    System.out.println(num1);
    System.out.println(num2);
    System.out.println(sum);
    // autofold {
  }
}
// }
```

The int can be declared and set in a similar way to the boolean.  Simply type the type of variable (`int`) and then the name of variable you'd like to create (`num1`).  Don't forget the semicolon.  To set the value, simply type an equals sign `=` followed by the desired value.

Notice that you can perform mathematical operations with int values.  You can use additon (`+`), subtraction (`-`), multiplication (`*`), or division (`/`) to perform mathemtical operations on your numbers.  There are a few more math operations that we'll get into later.

Try running the code above and see how it behaves.  Try changing some of the numbers in the code and see how the output changes.  Feel free to experiment with the code and see how it works.

#### double

INCOMPLETE, WILL BE FINISHED LATER

#### byte

#### short

#### long

#### float

### char

## String

## Other non-primative variables

# Phew!

Congratulations, you've made it through the variables lesson!  As you can probably tell, variables are a vital part of any programming language.  Without the variables, programs wouldn't be able to store any data or perform meaningful tasks.

Let's review your newly aquired skills in this quick quiz on the next page.

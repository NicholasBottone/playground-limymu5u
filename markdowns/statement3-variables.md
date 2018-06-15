# Variables

You may recall on the last activity we briefly mentioned **variables**.  We're going to take an in depth look at variables right now.

## What is a variable?

A **variable** is a value that can change, depending on conditions or on information passed to the program. Typically, a program consists of instructions that tell the computer what to do and data that the program uses when it is running.

You can think of a variable as a container or bin that can hold hold little pieces of information and data.  A variable could hold a **number**, a **letter**, a **word**, a **sentence**, or plenty of other types of data.

## Types of Primative Variables

There are eight primative types of variables used in Java, each of which serving distinct purposes.

### boolean

The simplest, most basic type of variable is called a `boolean`.  The boolean variable can only have two states: `true` or `false`.  

The boolean variable is **binary** -- that is, it only has two states.  It is either **on** or it is **off**.  It is either **1** or it is **0**.  `true` or `false`.

```java runnable
// { autofold
public class Main {
  public static void main(String[] args) {
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
// { autofold
public class Main {
  public static void main(String[] args) {
    // }
    int num1 = 3;
    int num2 = 6;
    int sum = num1 + num2;
    
    System.out.println(num1);
    System.out.println(num2);
    System.out.println(sum);
    // { autofold
  }
}
// }
```

The int can be declared and set in a similar way to the boolean.  Simply type the type of variable (`int`) and then the name of variable you'd like to create (`num1`).  Don't forget the semicolon.  To set the value, simply type an equals sign `=` followed by the desired value.

Notice that you can perform mathematical operations with int values.  You can use addition (`+`), subtraction (`-`), multiplication (`*`), or division (`/`) to perform mathemtical operations on your numbers.  There are a few more math operations that we'll get into later.

Try running the code above and see how it behaves.  Try changing some of the numbers in the code and see how the output changes.  Feel free to experiment with the code and see how it works.

#### double

A complex number which can contain many decimal places is a double (`double`).  A `double` variable can be positive or negative.  Like the `int`, there is also a limit to the size of the number that can be held, and there is also a limit to the number of decimal places the number can go to.  Doubles can be even larger (or smaller) than ints, so you don't have to worry about running out of room.

```java runnable
// { autofold
public class Main {
  public static void main(String[] args) {
    // }
    double firstDouble = 1.93;
    double secondDouble = 8.2;
    double thirdDouble = firstDouble + secondDouble;
    double fourthDouble = thirdDouble / 2;
    
    System.out.println(firstDouble);
    System.out.println(secondDouble);
    System.out.println(thirdDouble);
    System.out.println(fourthDouble);
    // { autofold
  }
}
// }
```

The double can be declared in a way similar to the int.  Just type the type of variable (`double`) followed by the name of the variable (`firstDouble`) and ending the line with a semicolon.  Use an equals sign after naming the variable to set the value of the variable, just like the int and boolean.

You can also perform mathematical operations with double values, just like with ints.  Use the same operators to add, subtract, multiply, or divide.  Note that when performing division, the double will be more accurate than the int since the double can contain decimals and fractions, while the int cannot.  

Try running the code above and see how it behaves.  Try changing some of the numbers and mathematical operators in the code and see how the output changes.  Feel free to experiment with the code and see how it works.

### char

The `char` is a unique type of variable.  `char` variables can hold one single **character**.  A character is any letter, number, or symbol that can be typed on your keyboard.  A `char` can hold singular letters like `'A'` or `'B'`, it can hold single-digit numbers like `'2'` or `'5'`, and finally it could hold singular symbols like `'@'` or `'/'`.  It is important to remember that a `char` can only hold **one character at a time**.  It cannot hold an entire word, phrase, or sentence.

The `char` can be defined using single quotes. (`'*'`)

```java runnable
// { autofold
public class Main {
  public static void main(String[] args) {
    // }
    char thisIsAChar = 'H';
    char anotherChar = 'I';
    char yetAnotherChar = '!';
    char charsAreCool = ' ';
    
    System.out.println(thisIsAChar);
    System.out.println(anotherChar);
    System.out.println(yetAnotherChar);
    System.out.println(charsAreCool);
    // { autofold
  }
}
// }
```

### Other primatives

There are a few other types of primative variables, although they are rarely used and are not very important for us to learn right now.  These primative variable types include the `byte`, `short`, `float`, and `long`.  These each can hold numberals, just like the int and double, but they each have different limitations for the smallest and largest numbers that they can hold.  A `float` can hold a low accuracy decimal, and the others each hold integers.

## String

A `String` is a very important type of variable.  Notice that the `String` variable is not a primative variable.  Any variable that begins with a capital letter is not of the primative type.  Nonprimative variables belong to classes.  Somewhere in the Java language library, there is a class that defines the String variable.  We do not have to worry about the code that makes the String work, because it is already done for us.  Since the nonprimative `String` is defined by a class, it cna have methods applied to it.  These methods can check or manipulate the data within the variable.

A `String` is important because it can hold any form of text.  This text could potentially be a number, a group of numbers, a word, a phrase, a sentence, or a paragraph.  **There is no limit to the size of a `String` variable**, therefore, you could potentially store the contents of an entire novel within a `String` variable if you so desired.  The only limitation to the size of a `String` is the amount of memory in the computer, which is not usually something you have to worry about.

The `String` can hold special characters just like the `char`, and it can even be empty.  To define a `String`, surround it with double quotes (quotation marks).  (`"HOORAY!"`)

```java runnable
// { autofold
public class Main {
    public static void main(String[] args) {
    // }
        String myString = "This is my string.";
        String yourString = "This is your string.";
        String emptyString = "";
        String paragraph = "According to all known laws of aviation, there is no way a bee should be able to fly. Its wings are too small to get its fat little body off the ground. The bee, of course, flies anyway because bees don't care what humans think is impossible.";
        
        System.out.println(myString);
        System.out.println(yourString);
        System.out.println(emptyString);
        System.out.println(paragraph);
        // { autofold
    }
}
// }
```

## Arrays

## Other non-primative variables

# Phew!

Congratulations, you've made it through the variables lesson!  As you can probably tell, variables are a vital part of any programming language.  Without the variables, programs wouldn't be able to store any data or perform meaningful tasks.

Let's review your newly aquired skills in this quick quiz on the next page.

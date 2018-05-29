# Hello World!

Let's jump right in and create your first program!
It can seem a little bit overwhelming at first, but don't worry, you'll be guided through the process step by step.

## The Goal

The goal of the application that we about to write is very simple.  We are going to create a Java class and method that will print a custom message back to the user after being run.  A Java Class is a file containing multiple pieces of code.  You can have many classes in an applications, but for this simple project, we'll just have one.  A Java method is a script that the programmer can call to run a predefined set of tasks and procedures.  We'll be creating a method that greets the user after running the command.

## Creating a class

```java
public class Main {
  
}
```

The very first thing we'll need to do is create a Java class.  For the sake of simplicity, let's name our class `Main`.
What you'll notice is that the Main class has two **modifiers** in front of it: `public` and `class`.

The `class` modifier lets the computer know that we are about to start defining a class object.
All of our code goes inside of a class object.  You can create many, many class objects in more complex programs, but we'll get to that later.

The `public` modifier tells the computer that the code in this class is going to be accessible from other classes that we code later.
We're not going to be creating any more classes yet, but it's always a good idea to use the public tag.
You can also use the `private` modifier, which means the code in this class cannot be accessed from other classes, or you could add no modifier at all, which only allows classes within the same folder or package to access the code in this class.

You'll notice that after declaring the class, we open and close these things called **curly brackets**.  `{ }`
You'll be using curly brackets often when coding in Java, so get used to them.
The curly brackets define what code is within an object.  In this case, all the code within the curly brackets belongs to the Main class.
There is no code within the curly brackets yet, so that means that no code belongs to the Main class yet.  Let's change that.

## Adding the main method

```java
public class Main {
  
  public static void main(String[] args) {
    
  }
  
}
```

Right off the bat, you'll notice that we've put something inside of the Main class.  This piece of code is called a **method**.
Methods are placed within classes, and they can hold several lines of code within them.
In this case, we are creating a method by the name of `main`.

Notice that like the class we created on the previous step, methods can have several modifiers.  
The `public` modifier allows the method to be accessed from other classes in the exact same way as the class.  
The `static` modifier tells the computer that this method does not use data that varies between several instances.  We'll get deeper into that later.  
The `void` modifier indicates that the method will not return anything back when it is called.  When you call a method, you can have it return a value (maybe a number or a word) back to the caller.  When a method is `void`, it does not return anything.

Notice the parentheses beside the name of the method.  `main(String[] args)`  
Inside the parentheses, all of the **arguments** are listed.  Arguments are **variables** that are passed on to the method when it is called.
A variable is a container that can hold a value.  There are several types of variables, and each type of variable each serves its own purpose.
Variables are very important in programming, and we'll go over them in the next activity.  For now, just understand that in order to call the `main` method, it is necessary to pass a single argument, specifically one of the type `String[]` named `args`.

After declaring the method and its arguments, we open and close the curly brackets once again. `{ }`  
All the code for this method will go inside of this method.  There's nothing in the method yet, so let's change that now.

## Printing to the console

```java runnable
public class Main {
  
  public static void main(String[] args) {
    
    System.out.println("Greetings, human.  I am a robot.  Hello world.");
    
  }
  
}
```

Now comes the exciting part!  The new code shown above will actually return a message back to the user's console!  Let's break it down.

`System` is actually the name of a public class that we are referencing.  The `System` class contains many useful commands and methods within it, but for this step, we'll be utilizing it to print a message to the console.

`out.println` is calling a method within the `System` class.  The `println` method takes one argument, and it is the message to be sent back to the user.  The message is denoted by quotation marks `" "`.

Notice that whenever you call a method or complete another task in Java, you should *always* end the line with a **semicolon**.  `;`  
The semicolon in Java is comparable to a period in English.  At the end of every line in Java, don't forget your punctuation.  Don't forget the semicolon!  `;`

Try pressing the run button below the code above!  What is the output?  
You should see a message that reads "Greetings, human.  I am a robot.  Hello world."  
This is the same message that is provided as an argument in the `println` method!

When you press the run button, your browser actually calls the method that we just created.  
If we wanted to do this in code, we could call our code by typing `Main.main(args);`

### **Try changing the message!**

That "Greetings, human..." message that we printed isn't the only thing we can use the `println` method for!  
Click on the code snippet above and edit the message to whatever you want, then press the run button again and see how it affects the result!  
Try changing it to `System.out.println("Beep boop I'm a bot");` or your name -- or whatever you'd like!

## Congratulations!

You've just made your first program!  Yes, it's simple, but by reusing the code we just wrote, we can print all sorts of messages to the console.

The "Hello World" program is a traditional introductory program for beginners to make.
We're going to make more advanced programs - and even a few basic games.  But first, let's review what you've learned in a basic quiz.

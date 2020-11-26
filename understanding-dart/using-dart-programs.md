---
description: How do we use Dart programs? How does Dart use our code?
---

# Using Dart Programs

## Non-primitive data types

One of the most basic code statements you can write in Dart is as follows:

```java
int i = 0;
```

This declares the variable `i` with the data type `int` and a value of `0`. Integers are primitive data types, but what happens when we use non-primitive data types?

Let's say that we make a class, `LightBulb`. \(Don't worry about that terminology for now, just focus on the theory!\) How would we use `LightBulb` as a data type and pass it as a value?

```java
LightBulb light = new LightBulb();
```

You can see that we are essentially creating a "new" LightBulb to be stored by the variable `light`. Not much syntax changed on the left hand side, but on the right hand side things are different. Here, we are making a `new` light bulb, instead of just typing something like `0` for an integer or `"hi"` for a String.

## Client of the class

By creating a "new" object, we are now a _client_ of a class. In the case of the `LightBulb` class, we are a "client" of the class LightBulb, and must use the methods accordingly.

Being a _client_ of a class or another program means that we are able to use parts of code without actually having to know how it works, as long as we know what it does. For example, consider a computer: we know that it should run and operate, but it doesn't matter exactly how it does it as long as it does it.

This works the same way for the `LightBulb` class. Say we can turn our `light` on and off with the methods `turnOn()` and `turnOff()`. We can call these methods like `light.turnOn()` and we know exactly what they will do, but we don't need to understand how they work in order to use them in our own code.

## Printing to console

Sometimes, we will need to debug our code. If there is something that isn't working properly, or we need to keep track of something while we are coding, we can use the `print` method. This will print text to the console, or the right-hand side of the screen on [DartPad](https://dartpad.dev).

We can use the `print` method like so:

```dart
print("Hello console!");
```

## Main function

Every Dart program must have a `main` method. This tells Dart where to begin the program. We will learn more about methods in a later lesson, but this is what a basic `main` method looks like.

```dart
void main() {
    print("Hello");
}
```


# Flutter

## Dart

Dart is an open-source, general-purpose, object-oriented programming language with C-style syntax developed by Google in 2011. The purpose of Dart programming is to create a frontend user interfaces for the web and mobile apps. It can also be used to build server and desktop applications.

### Variables

- #### variable declaration using `var`

There are different ways to initialize a variable in Dart. The straight forward and recommended way is by using the keyword `var`.

```dart
    var personName = 'John Doe';
    var personAge = 25;
```

Based on the value assigned into a variable, Dart will automatically infer data type to that variable. In the above example, Dart will automatically give the type of `String` to personName and `int` to personAge.

After initializing a variable with certain type of data using **var** keyword, it is not possible to assign a different type of data in the same variable later.

Suppose if we try to assign `personName = 123`  we get the following error message

>*“A value of type ‘int’ can’t be assigned to a variable of type `String`"*

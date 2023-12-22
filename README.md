# Flutter

## Dart

Dart is an open-source, general-purpose, object-oriented programming language with C-style syntax developed by Google in 2011. The purpose of Dart programming is to create a frontend user interfaces for the web and mobile apps. It can also be used to build server and desktop applications.

### Basic structure to execute Dart file

```dart
void main(){
    // code goes here
}
```

### Variables

- #### **Variable declaration using `var`**

There are different ways to initialize a variable in Dart. The straight forward and recommended way is by using the keyword `var`.

```dart
    var personName = 'John Doe';
    var personAge = 25;
```

Based on the value assigned into a variable, Dart will automatically infer data type to that variable. In the above example, Dart will automatically give the type of `String` to personName and `int` to personAge.

After initializing a variable with certain type of data using **var** keyword, it is not possible to assign a different type of data in the same variable later.

Suppose if we try to assign `personName = 123`  we get the following error message

>*“A value of type ‘int’ can’t be assigned to a variable of type `String`"*

- #### **Variable declaration using `Object` or `dyanmic`**

unlike `var` keyword we can fit in any data type to variables using `Object` and `dynamic`

`Object` and `dynamic` keywords are often understood as inter-changable.

Example: 

```dart
// Using object
void main(){
  Object objvar = "John Doe";
  print(objvar);
  objvar = 124;
  print(objvar);
}
```

```dart
// Using dynamic
void main(){
  dynamic dynvar = "John Doe";
  print(dynvar);
  dynvar = 124;
  print(dynvar);
}
```

Here both keywords will give same output:
> John Doe <br> 124

#### Key differences between `dyanmic` and `Object`

>**Note!!!** <br>
Eventhough they show the same output, they are usually not interchangeable.

In Dart, `dynamic` and `Object` are both types that can hold values of any type. However, they have some key differences:

| **dynamic**            | **Object** |
|--------------------|----------------------------|
| `dynamic` is a type that tells the Dart compiler to skip type checking at compile time. This means that the type of a dynamic variable can be determined at runtime. | `Object` is a class in Dart's core library. It is the root of the Dart class hierarchy and is a supertype of all Dart types, meaning every class and data types are extended from Object. When you use Object, you still have to adhere to Dart's static typing rules, which means you have to perform explicit type conversions when necessary. |

- #### Variable Declaration using Data Type

There are several built-in data types, including:

`int`: used to store integers<br>
`double`: used to store floating-point numbers<br>
`String`: used to store text<br>
`bool`: used to store true or false value<br>
`List`: used to store ordered collections of objects<br>
`Map`: used to store unordered collections of key-value pairs<br>
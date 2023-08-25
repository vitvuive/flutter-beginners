# Flutter for Beginner

# Section 1: Introduction to Dart

### Fuchsia OS

Google has been working on a new operating system called Fuchsia OS which has been remoted to be a potential future replacement for the Android OS.

The growth of the framework's adoption is directly related to the new Fuchsia OS. As it gets closer to launch. It's importance to Google to have apps targeting the new system. For example Google announced that Android apps will be compatible with the new OS, making the transition to, and adoption of Flutter significantly easier.

### Flutter hight performance

- Flutter owns the pixels: Flutter renders the application pixel by pixel, interacting directly with the Skia Graphics engine.
- No extra layers or additional OS API calls: As Flutter owns the app rendering, It does not need additional calls to use the OEM widgets, no no bottleneck.
- Flutter is compiled to native code: Flutter uses the Dart AOT compiler to produce native code. That means there's no over head in setting up an environment to interpret Dart code on the fly. and it runs just like a native app. Starting more quickly than frameworks that need some kind of interpreter.

## Full control of the UI

- Ruling all the pixels on the device
- Platform UI kit
- Achievable UI deisn requirement
- Smoother look and feel

## Building and running Flutter

- Debug mode
- Release mode

> Skia graphics library. Skia is an open source library that provides APIs for 2D graphics. It is used in Flutter as well as Google Chrome, Android, Firefox, and many others. It is also backed by Google, like Dart and Flutter.

- Profile mode

### The pubspec.yaml file

# An Introducation to Dart

### Dart VM and Javascript compilation

The execution of Dart code in operates in two modes (Just In Time) JIT compilation or (Ahead of Time) AOT compilation.

- a JIT compilation is where the source code is compiled as it is needed - just in time. The Dart VM loads and compiles the source code to native machine code on the fly. This approach is used to run code on the command line or during mobile application develop to allow the use of features such as debugging and hot reload.
- An AOT compilation is where the Dart VM and your code are precompiled and the VM works more like a Dart runtime system, providing a garbage collector and the various native methods from the Dart software development kit (SDK) to the application. This approach has huge performance benefits over JIT compilations but other features such as debugging and hot reload are not available.

## Introducing the structure of the Dart language

### Object orientation

### Dart operators

### Variable Declaration

#### Null safety

- ?
- `late`
- Null aware methods

#### Number

`int`

`double`

#### Booleans

#### Lists

#### Maps

#### Strings

#### Const and final

# Flutter versus Other Frameworks

## Moving to Flutter from React Native

Key differences between JS and Dart:

- Variables: Unlike JS, Dart is a type safe languages, so variables must be declared with a type or the type system can infer the type.
- Dart has no concept of undefined. Either a variable of true or it is null.
- Dart has no concept of truthy. Only the Boolean value of true is treated as a true value.
- The JS Promise is represented by Dart Future object. The async and await operator act on Futures like the do on Promise in JS.
- Printing to the console uses the print method insteads console.log()

# Dart Classes and Constructs

## Object orientation in Dart

#### Objects and Classes

#### Other OOP artifacts

#### Encapsulation (Dong Goi)

#### Inheritance and composition (Ke Thua va Thanh Phan)

#### Abstraction

#### Polymorphism (Da Hinh)

#### Functions as objects

## Unstanding claases in Object

### Class structure

- Field
- Accessors
- Constructor
- Methods

#### Field accessors - getters and setters

#### Static fields and methods

#### Constructors

- Named constructors
- Factory constructors

#### Class inheritance

#### Abstract classes

Must have, if it did not, the class would itself be abstract and therefore could not be instantiated.

#### Interface

Dart has **implicit interfaces**

#### Mixins

```
class SeniorDeveloper extends Person with ProgrammingSkills,
ManagementSkills
```

### Files and import

### The enum type

```
  enum PersonType { student, employee }
```

### Using generics

`<>`

#### When and Why to use generics

The use of generics can help a developer to maintain and keep collection behavior under control.

When we use a collection without specifying the allowed element types, it is our responsibility to correctly insert elements of the expected type. This can lead to bugs when data of an incorrect type is placed in a collection or incorrect assumptions are made about the contents of a collection.

#### Asynchronous programming

Dart is a single-threaded programming language.

`sleep`

`delayed`

## Dart Isolates

Isolates allow the main function runs ahead of the function.

# Section 2: The Flutter User Interface Everything Is a Widget

#### Statefull/Stateless Widget

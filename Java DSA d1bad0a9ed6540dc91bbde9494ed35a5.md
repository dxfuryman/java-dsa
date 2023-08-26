# Java DSA

![Untitled](Java%20DSA%20d1bad0a9ed6540dc91bbde9494ed35a5/Untitled.png)

## First class Functions :

In computer programming, the term "first-class" typically refers to the concept of first-class functions or first-class citizens. This concept is found in programming languages that treat functions as first-class citizens, meaning that functions are treated like any other data types, such as integers or strings. Here are the main characteristics or functions of first-class functions:

1. Assignability: First-class functions can be assigned to variables, just like other data types. This allows you to store functions as values and use them later in your code.
2. Passing as Arguments: You can pass first-class functions as arguments to other functions. This feature is particularly useful for implementing higher-order functions, which take other functions as parameters.
3. Return Value: First-class functions can be returned as the result of other functions. This enables the creation of more flexible and powerful abstractions in your code.
4. Stored in Data Structures: First-class functions can be stored in data structures such as arrays, lists, or dictionaries. This capability is crucial for creating data structures that contain a mixture of data and functions.
5. Anonymous Functions (Lambda Expressions): Some programming languages that support first-class functions also allow the creation of anonymous functions, often called lambda expressions. These functions do not require a formal name and can be used directly in expressions.
6. Higher-order Functions: First-class functions enable the existence of higher-order functions, which are functions that either take one or more functions as arguments or return a function as their result. Higher-order functions are a powerful programming paradigm that allows for more concise and expressive code.

Languages that support first-class functions include Python, JavaScript, Ruby, Lisp, and many others. The ability to use functions as first-class citizens provides a significant advantage in terms of code organization, reusability, and flexibility, allowing developers to implement more elegant and sophisticated solutions to various problems.

![Untitled](Java%20DSA%20d1bad0a9ed6540dc91bbde9494ed35a5/Untitled%201.png)

## In the computer memory management The variable we use is stored in  the stack memory and the object we use is stored in the heap memory

![Untitled](Java%20DSA%20d1bad0a9ed6540dc91bbde9494ed35a5/Untitled%202.png)

## note :

many reference variables can point or use a same object and if one ref variable changes the value of the object it will change the value for all the variables.

![Untitled](Java%20DSA%20d1bad0a9ed6540dc91bbde9494ed35a5/Untitled%203.png)

## Garbage collection:

Objects which do not have any ref variable pointing towards them are known as garbage variables . Eventually they are removed from the memory .

![Untitled](Java%20DSA%20d1bad0a9ed6540dc91bbde9494ed35a5/Untitled%204.png)

suppose you write a=10 and again you write a=30 then what will happen to this 10 the garbage collection will come and remove it from the memory .

## Flowcharts :

![Untitled](Java%20DSA%20d1bad0a9ed6540dc91bbde9494ed35a5/Untitled%205.png)

## Psudo code :

it is like a rough code. 

![Untitled](Java%20DSA%20d1bad0a9ed6540dc91bbde9494ed35a5/Untitled%206.png)

# JAVA BASICS ➖

![Untitled](Java%20DSA%20d1bad0a9ed6540dc91bbde9494ed35a5/Untitled%207.png)

NOTE : In c and C++ the middle part is skiped and it directly compile the source code into machine code thats why JAVA is a platform independent language.

![Untitled](Java%20DSA%20d1bad0a9ed6540dc91bbde9494ed35a5/Untitled%208.png)

java actually converts the source code into byte code and then that byte code can bee used in any platforms whereas c++ converts it in .exe file which is platform dependent . 

# JDK :

![Untitled](Java%20DSA%20d1bad0a9ed6540dc91bbde9494ed35a5/Untitled%209.png)

Note : In do while loops the loop is going to execute atleast once and after that it will not excute until w00hile condition is true.

# Loops:

- **Loops** are used to repeat a block of code a certain number of times.
- Java has three types of loops: `for`, `while`, and `do-while`.
- The `for` loop is the most commonly used loop in Java. It has a specific syntax that allows you to initialize, test, and update a variable within the loop.
- The `while` loop is a simple loop that tests a condition before each iteration. If the condition is true, the loop body is executed. If the condition is false, the loop terminates.
- The `do-while` loop is similar to the `while` loop, except that the loop body is executed at least once, even if the condition is false.

Here is an example of a `for` loop in Java:

```java
for (int i = 0; i < 10; i++) {
  System.out.println(i);
}
```

This loop will print the numbers from 0 to 9. The `for` loop has three parts:

- The initialization expression: `int i = 0;` This expression initializes the variable `i` to 0.
- The condition: `i < 10;` This expression tests whether `i` is less than 10. If it is, the loop body is executed. If it is not, the loop terminates.
- The update expression: `i++;` This expression increments the value of `i` by 1.

Here is an example of a `while` loop in Java:

```java
int i = 0;
while (i < 10) {
  System.out.println(i);
  i++;
}
```

This loop is similar to the `for` loop, except that the condition is checked before each iteration. The loop body is only executed if the condition is true.

Here is an example of a `do-while` loop in Java:

```java
int i = 0;
do {
  System.out.println(i);
  i++;
} while (i < 10);
```

This loop is similar to the `while` loop, except that the loop body is executed at least once, even if the condition is false. The condition is checked after the loop body is executed.

## Switch case :

![Untitled](Java%20DSA%20d1bad0a9ed6540dc91bbde9494ed35a5/Untitled%2010.png)

If break condition is not there the it will run all the conditions beneath it .

## Note: Why we use static in PSVM?

The keyword `static` in `public static void main()` means that the `main()` method is a **static method**. A static method is a method that belongs to the class itself, rather than to any specific instance of the class. This means that there is only one copy of the `main()` method in memory, regardless of how many instances of the class are created.

The `main()` method is always static in Java because it is the entry point for the Java program. When the Java Virtual Machine (JVM) starts a Java program, it looks for the `main()` method in the class that is specified as the main class. The JVM then calls the `main()` method, and the program starts executing.

The `static` keyword also has other implications for the `main()` method. For example, static methods cannot access instance variables or methods, because these variables and methods are not available to the class itself.

# Functions in JAVA :

```java
public static void main(String[] args) {
        sum();
    }
    static void sum() {
        Scanner in=new Scanner(System.in);
        System.out.println("Enter num1");
        int num1= in.nextInt();
        System.out.println("Enter num2");
        int num2=in.nextInt();
        int add =num1+num2;
        System.out.println(add);
    }
```

In this we created a function sum and than call it and give its values and defination outside the main function because main function will be called first .

## In intellij idea we use shortcut Alt + Enter  to enhance a code or to create a function class .

## Note : You can never modify strings due to security reasons.

# Scoping:

Scoping in Java refers to the area where a variable or method is visible and accessible to other code. There are three main types of scope in Java:

- **Method scope:** Variables declared directly inside a method are available anywhere in the method following the line of code in which they were declared.
- **Block scope:** A block of code refers to all of the code between curly braces {}. Variables declared inside blocks of code are only accessible by the code between the curly braces, which follows the line in which the variable was declared.
- **Class scope:** Variables declared within a class are accessible by all methods in that class. Depending on its access modifier (ie. public or private), it can sometimes be accessed outside the class.

For example, the following code shows a variable declared with method scope:

**Java**

```java
public class MyClass {

    public void myMethod() {
        int myVariable = 10;
        System.out.println(myVariable);
    }
}

```

**Use code with caution. [Learn more](https://bard.google.com/faq#coding)content_copy**

The variable `myVariable` is only accessible inside the `myMethod()` method. If you try to access it outside of the method, you will get a compiler error.

The following code shows a variable declared with block scope:

**Java**

```java
public class MyClass {

    public void myMethod() {
        int myVariable = 10;
        {
            int anotherVariable = 20;
            System.out.println(myVariable);
            System.out.println(anotherVariable);
        }
        // anotherVariable is not accessible here
    }
}

```

**Use code with caution. [Learn more](https://bard.google.com/faq#coding)content_copy**

The variable `anotherVariable` is only accessible inside the block of code where it is declared. If you try to access it outside of the block, you will get a compiler error.

The following code shows a variable declared with class scope:

**Java**

```java
public class MyClass {

    int myVariable = 10;

    public void myMethod() {
        System.out.println(myVariable);
    }
}

```

The variable `myVariable` is accessible inside the `MyClass` class, including all of its methods. You can also access it from outside the class, as long as you have the appropriate access modifier.

## Anything that is used outside the block can be used inside the block but anything used inside the block can’t be used outside the block.

## Shadowing:

![Untitled](Java%20DSA%20d1bad0a9ed6540dc91bbde9494ed35a5/Untitled%2011.png)

In this the x=90 is shadowed and x=40 will have more priority than the upper x . In this the lower level x is over riding the upper level x this is known as shadowing.

→ you will have to initialize the value of the variable before using it f

![Untitled](Java%20DSA%20d1bad0a9ed6540dc91bbde9494ed35a5/Untitled%2012.png)

## Variable length arguments [VarArgs] :

In this we can take any number of values and the compiler will automatically convert it into array and store the value in it.

![Untitled](Java%20DSA%20d1bad0a9ed6540dc91bbde9494ed35a5/Untitled%2013.png)

Output:

![Untitled](Java%20DSA%20d1bad0a9ed6540dc91bbde9494ed35a5/Untitled%2014.png)

For multiple arguments we can also use

 

![Untitled](Java%20DSA%20d1bad0a9ed6540dc91bbde9494ed35a5/Untitled%2015.png)

## Function overloading:

In this situation there are functions with same name but different parameters. It means ➖

![Untitled](Java%20DSA%20d1bad0a9ed6540dc91bbde9494ed35a5/Untitled%2016.png)

## Ambiguity:

Ambiguity in Java varargs occurs when there are two or more overloaded methods that can be called with the same number of arguments, including the varargs argument. The compiler cannot determine which method to call, and will generate an error.

# Arrays➖

Array is a collection of similar type of data type .All the type of data in the array should be same 

![Untitled](Java%20DSA%20d1bad0a9ed6540dc91bbde9494ed35a5/Untitled%2017.png)

![Untitled](Java%20DSA%20d1bad0a9ed6540dc91bbde9494ed35a5/Untitled%2018.png)

## Now lets understand the mechanism of arrays

![Untitled](Java%20DSA%20d1bad0a9ed6540dc91bbde9494ed35a5/Untitled%2019.png)

It follows Dynamic memory allocation because its memory is assigned at the run time .

### Note : new is used to create an object.

How to input values in arrays:

![Untitled](Java%20DSA%20d1bad0a9ed6540dc91bbde9494ed35a5/Untitled%2020.png)

![Untitled](Java%20DSA%20d1bad0a9ed6540dc91bbde9494ed35a5/Untitled%2021.png)

The `Arrays.toString()` method in Java is a static method that belongs to the `java.util` package. It is used to convert an array to a string representation. The string representation consists of a list of the array's elements, enclosed in square brackets ("[]"). Adjacent elements are separated by the characters ", " (a comma followed by a space).

```java
int[] array = {1, 2, 3, 4, 5};
System.out.println(Arrays.toString(array));
```

## Multi dimensional Arrays ➖

![Untitled](Java%20DSA%20d1bad0a9ed6540dc91bbde9494ed35a5/Untitled%2022.png)

Here in new int[3][4] the first array column is used for the rows and second is used for the column .

row column should contain a value whereas column can be leaved empty .

For input with loops we use a particular logic for example:

![Untitled](Java%20DSA%20d1bad0a9ed6540dc91bbde9494ed35a5/Untitled%2023.png)

## Introduction to Array list ➖

![Untitled](Java%20DSA%20d1bad0a9ed6540dc91bbde9494ed35a5/Untitled%2024.png)

Using list elements :

![Untitled](Java%20DSA%20d1bad0a9ed6540dc91bbde9494ed35a5/Untitled%2025.png)

![Untitled](Java%20DSA%20d1bad0a9ed6540dc91bbde9494ed35a5/Untitled%2026.png)

![Untitled](Java%20DSA%20d1bad0a9ed6540dc91bbde9494ed35a5/Untitled%2027.png)

Lets see how it works internally:

Actually what happens lets suppose your array is having 3 elements and if want to add another element to it than it will copy the elements of this array and double the size of this array and paste it to new array created and than you can add the fourth element and the old array will be deleted

![Untitled](Java%20DSA%20d1bad0a9ed6540dc91bbde9494ed35a5/Untitled%2028.png)

![Untitled](Java%20DSA%20d1bad0a9ed6540dc91bbde9494ed35a5/Untitled%2029.png)

## How to print multidimensional array list.

![Untitled](Java%20DSA%20d1bad0a9ed6540dc91bbde9494ed35a5/Untitled%2030.png)

![Untitled](Java%20DSA%20d1bad0a9ed6540dc91bbde9494ed35a5/Untitled%2031.png)

- QUESTIONS OF ARRAYS➖
    - Reversing array using  Swapping two numbers ➖
        
        ### Reversing array using Swapping two numbers ➖
        
        ```java
        import java.util.Arrays;
        
        public class Main {
            public static void main(String[] args) {
                int[] arr = {1, 2, 3, 4, 5};
                System.out.println("Original array: " + Arrays.toString(arr));
                reverseArray(arr);
                System.out.println("Reversed array: " + Arrays.toString(arr));
            }
        
            static void reverseArray(int[] arr) {
                int start = 0;
                int end = arr.length - 1;
                while (start < end) {
                    int temp = arr[start];
                    arr[start] = arr[end];
                    arr[end] = temp;
                    start++;
                    end--;
                }
            }
        }
        
        ```
        
        The code first creates an integer array named `arr` with the elements 1, 2, 3, 4, and 5. It then prints the original array to the console.
        
        The next step is to call the `reverseArray()` method. This method takes the `arr` array as its input parameter. The method first defines two variables, `start` and `end`. The `start` variable is initialized to 0, and the `end` variable is initialized to the length of the array minus 1.
        
        The method then enters a loop. The loop will continue as long as `start` is less than `end`. Inside the loop, the method does the following:
        
        - It creates a temporary variable and stores the value of `arr[start]` in it.
        - It then sets `arr[start]` to the value of `arr[end]`.
        - It then sets `arr[end]` to the value of the temporary variable.
        - Finally, it increments `start` by 1 and decrements `end` by 1.
        
        This process reverses the order of the elements in the array.
        
        The last step in the code is to call the `reverseArray()` method again. This time, the reversed array is printed to the console.
        
        Here is the output of the code:
        
        `Original array: [1, 2, 3, 4, 5] Reversed array: [5, 4, 3, 2, 1]`
        
    - Char to array of characters
        
        ```java
        public class StringToCharacterArray {
        
            public static void main(String[] args) {
                String str = "Hello";
                char[] chArray = str.toCharArray();
                System.out.println(Arrays.toString(chArray)); // [H, E, L, L, O]
            }
        }
        
        ```
        
        The `toCharArray()` method of the `String` class converts the string to a character array. The method returns a new character array that contains the characters of the string. The length of the character array is the same as the length of the string.
        
        In the code above, we first create a string variable named `str` and initialize it to the value "Hello". We then call the `toCharArray()` method on `str` and store the result in a character array variable named `chArray`. Finally, we print the elements of the character array using the `Arrays.toString()` method.
        
        The output of the code is:
        
        `[H, E, L, L, O]`
        
    - 

## Constants in JAVA➖

The Integer class in Java has the following constants:

- **MAX_VALUE:** The maximum value that an integer variable of the int data type can hold. The value of MAX_VALUE is 2147483647.
- **MIN_VALUE:** The minimum value that an integer variable of the int data type can hold. The value of MIN_VALUE is -2147483648.
- **SIZE:** The number of bits used to represent an integer variable of the int data type. The value of SIZE is 32.
- **TYPE:** The data type of an integer variable. The value of TYPE is int.

In addition to these constants, the Integer class also has a number of methods for converting between strings and integers, and for performing mathematical operations on integers.

Here is a table of all the constants in the Integer class:

| Constant | Value | Description |
| --- | --- | --- |
| MAX_VALUE | 2147483647 | The maximum value that an integer variable of the int data type can hold. |
| MIN_VALUE | -2147483648 | The minimum value that an integer variable of the int data type can hold. |
| SIZE | 32 | The number of bits used to represent an integer variable of the int data type. |
| TYPE | int | The data type of an integer variable. |
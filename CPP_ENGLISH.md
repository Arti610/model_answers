1. **Define C language, features, and application of it.**
   - **C Language:** C is a general-purpose, procedural programming language developed by Dennis Ritchie at Bell Labs in the early 1970s. It is widely used for developing system software, applications, and embedded systems.
   - **Features of C:**
     - Simple and efficient syntax.
     - Low-level manipulation of data.
     - Direct access to memory.
     - Extensive library support.
     - Modularity and reusability.
   - **Applications of C:**
     - Operating systems development.
     - Embedded systems programming.
     - Game development.
     - Compiler construction.
     - System utilities.

2. **Define the following:**
   - **Compiler:** A compiler is a program that translates the entire source code of a program written in a high-level programming language into machine code or an intermediate code. It performs analysis and optimization before generating the executable code.
   - **Interpreter:** An interpreter is a program that directly executes the source code of a program line by line. It translates and executes each statement one at a time without generating a separate executable file.
   - **Assembler:** An assembler is a program that translates assembly language code into machine code. It converts symbolic instructions and addresses into binary code that can be executed by a computer's central processing unit (CPU).
   - **Variable:** A variable is a named storage location in a program where data can be stored and manipulated. It has a specific data type and a unique identifier.
   - **Identifier:** An identifier is a name given to a variable, function, class, or any other user-defined item in a program. It follows specific rules and conventions.
   - **Literal:** A literal is a constant value used in a program, such as numbers, characters, or strings, whose value does not change during program execution.

- **Data type:**
   - A data type is a classification that specifies which type of value a variable can hold. It defines the operations that can be performed on the data, the meaning of the data, and the way values of that type can be stored.

- **Operator:**
   - An operator is a symbol that represents a specific operation performed on one or more operands. Examples include arithmetic operators (+, -, *, /), relational operators (<, >, ==), and logical operators (&&, ||).

- **Control statements with syntax:**
   - Control statements are used to manage the flow of execution in a program. Examples include if-else, switch, for loop, while loop, and do-while loop.

- **Class:**
   - In object-oriented programming (OOP), a class is a blueprint or template for creating objects. It defines the properties and behaviors common to all objects of that type.

- **Object, how to create an object:**
   - An object is an instance of a class. To create an object in C++, you use the following syntax:
     ```cpp
     ClassName objectName;
     ```

- **Encapsulation:**
   - Encapsulation is the bundling of data and the methods that operate on that data into a single unit called a class. It helps in hiding the internal implementation details from the outside world.

- **Data Abstraction:**
   - Data abstraction is the concept of hiding the complex implementation details and showing only the essential features of an object. It involves defining a class interface without revealing its internal workings.

- **Differentiate OOPs vs POPs:**
    - Object-oriented programming (OOP) focuses on organizing code into classes and objects, promoting concepts like encapsulation, inheritance, and polymorphism. Procedural programming (POP) is centered around procedures or routines.

- **Define “Recursion” with a program:**
    - Recursion is a programming technique where a function calls itself. Example in C++:
      ```cpp
      #include <iostream>
      using namespace std;

      int factorial(int n) {
          if (n == 0 || n == 1)
              return 1;
          else
              return n * factorial(n - 1);
      }

      int main() {
          int num = 5;
          cout << "Factorial of " << num << " is " << factorial(num) << endl;
          return 0;
      }
      ```

- **Constructor and destructor:**
    - **Constructor:** A constructor is a special member function in a class that is automatically called when an object is created. It is used for initializing the object's data members.
    - **Destructor:** A destructor is a special member function in a class that is automatically called when an object goes out of scope or is explicitly deleted. It is used for cleanup tasks.

- **Inheritance:**
    - Inheritance is an OOP concept where a class (subclass/derived class) inherits properties and behaviors from another class (superclass/base class). It promotes code reuse and supports the "is-a" relationship.

- **Friend function:**
    - A friend function is a function that is not a member of a class but is allowed to access its private and protected members. It is declared inside the class with the `friend` keyword.

- **Virtual function:**
    - A virtual function in C++ is a function declared in a base class that can be overridden in its derived classes. It enables dynamic polymorphism and allows the correct function to be called at runtime.

- **Inline function:**
    - An inline function is a function defined with the `inline` keyword. It suggests the compiler to insert the complete code of the function at the point of each function call, instead of performing a regular function call.

- **C++ Tokens:**
    - C++ tokens are the smallest units in the C++ programming language. They include keywords, identifiers, literals, operators, and special symbols. Examples include `int`, `variableName`, `123`, `+`, and `;`.



3. **C "Hello, World!" Program:**
   ```c
   #include <stdio.h>

   int main() {
       printf("Hello, World!\n");
       return 0;
   }
   ```

4. **C Program to Swap Two Numbers:**
   ```c
   #include <stdio.h>

   int main() {
       int num1, num2, temp;

       printf("Enter two numbers:\n");
       scanf("%d %d", &num1, &num2);

       // Swapping logic
       temp = num1;
       num1 = num2;
       num2 = temp;

       printf("After swapping: %d %d\n", num1, num2);

       return 0;
   }
   ```

5. **C Program to Check Whether a Number is Even or Odd:**
   ```c
   #include <stdio.h>

   int main() {
       int num;

       printf("Enter a number:\n");
       scanf("%d", &num);

       // Checking if the number is even or odd
       if (num % 2 == 0)
           printf("%d is even.\n", num);
       else
           printf("%d is odd.\n", num);

       return 0;
   }
   ```

6. **C Program to Calculate the Sum of Natural Numbers:**
   ```c
   #include <stdio.h>

   int main() {
       int n, sum = 0;

       printf("Enter a positive integer: ");
       scanf("%d", &n);

       // Calculating the sum of natural numbers
       for (int i = 1; i <= n; ++i) {
           sum += i;
       }

       printf("Sum of natural numbers from 1 to %d: %d\n", n, sum);

       return 0;
   }
   ```

7. **C Program to Display Fibonacci Sequence:**
   ```c
   #include <stdio.h>

   int main() {
       int n, first = 0, second = 1, next;

       printf("Enter the number of terms: ");
       scanf("%d", &n);

       printf("Fibonacci Sequence:\n");

       for (int i = 0; i < n; ++i) {
           printf("%d, ", first);
           next = first + second;
           first = second;
           second = next;
       }

       return 0;
   }
   ```

8. **C Program to Display Characters from A to Z Using Loop:**
   ```c
   #include <stdio.h>

   int main() {
       printf("Characters from A to Z:\n");

       for (char ch = 'A'; ch <= 'Z'; ++ch) {
           printf("%c ", ch);
       }

       return 0;
   }
   ```

9. **C Program to Check Whether a Number is Palindrome or Not:**
   ```c
   #include <stdio.h>

   int main() {
       int num, reversedNum = 0, originalNum, remainder;

       printf("Enter an integer: ");
       scanf("%d", &num);

       originalNum = num;

       // Reversing the number
       while (num != 0) {
           remainder = num % 10;
           reversedNum = reversedNum * 10 + remainder;
           num /= 10;
       }

       // Checking if the number is a palindrome
       if (originalNum == reversedNum)
           printf("%d is a palindrome.\n", originalNum);
       else
           printf("%d is not a palindrome.\n", originalNum);

       return 0;
   }
   ```

10. **C Program to Check Armstrong Number:**
    ```c
    #include <stdio.h>
    #include <math.h>

    int main() {
        int num, originalNum, remainder, n = 0, result = 0;

        printf("Enter an integer: ");
        scanf("%d", &num);

        originalNum = num;

        // Calculating the number of digits
        while (originalNum != 0) {
            originalNum /= 10;
            ++n;
        }

        originalNum = num;

        // Checking if the number is an Armstrong number
        while (originalNum != 0) {
            remainder = originalNum % 10;
            result += pow(remainder, n);
            originalNum /= 10;
        }

        if (result == num)
            printf("%d is an Armstrong number.\n", num);
        else
            printf("%d is not an Armstrong number.\n", num);

        return 0;
    }
    ```

11. **C Program to Make a Simple Calculator Using switch...case:**
    ```c
    #include <stdio.h>

    int main() {
        char operator;
        double num1, num2, result;

        printf("Enter an operator (+, -, *, /): ");
        scanf(" %c", &operator);

        printf("Enter two numbers: ");
        scanf("%lf %lf", &num1, &num2);

        switch (operator) {
            case '+':
                result = num1 + num2;
                break;
            case '-':
                result = num1 - num2;
                break;
            case '*':
                result = num1 * num2;
                break;
            case '/':
                if (num2 != 0)
                    result = num1 / num2;
                else {
                    printf("Error! Division by zero is not allowed.\n");
                    return 1; // Exit with an error code
                }
                break;
            default:
                printf("Error! Invalid operator.\n");
                return 1; // Exit with an error code
        }

        printf("Result: %.2lf %c %.2lf = %.2lf\n", num1, operator, num2, result);

        return 0;
    }
    ```

12. **C++ "Hello, World!”:**
    ```cpp
    #include <iostream>

    int main() {
        std::cout << "Hello, World!" << std::endl;
        return 0;
    }
    ```

Certainly! Here's a C program to print a half-pyramid using `*`:

```c
#include <stdio.h>

int main() {
    int rows;

    printf("Enter the number of rows: ");
    scanf("%d", &rows);

    for (int i = 1; i <= rows; ++i) {
        for (int j = 1; j <= i; ++j) {
            printf("* ");
        }
        printf("\n");
    }

    return 0;
}
```

This program prompts the user to enter the number of rows for the half-pyramid and then prints the pattern using asterisks (`*`). Each row has an increasing number of asterisks, forming a half-pyramid pattern.

Certainly! Here's a C program to print a half-pyramid using alphabets:

```c
#include <stdio.h>

int main() {
    int rows;
    char currentChar = 'A';

    printf("Enter the number of rows: ");
    scanf("%d", &rows);

    for (int i = 1; i <= rows; ++i) {
        for (int j = 1; j <= i; ++j) {
            printf("%c ", currentChar);
        }
        ++currentChar;
        printf("\n");
    }

    return 0;
}
```

This program prompts the user to enter the number of rows for the half-pyramid and then prints the pattern using alphabets (starting from 'A'). Each row has an increasing number of alphabets, forming a half-pyramid pattern.

Certainly! Here's a C program to print a full pyramid pattern using `*`:

```c
#include <stdio.h>

int main() {
    int rows;

    printf("Enter the number of rows: ");
    scanf("%d", &rows);

    for (int i = 1, k = 0; i <= rows; ++i, k = 0) {
        for (int space = 1; space <= rows - i; ++space) {
            printf("  ");
        }

        while (k != 2 * i - 1) {
            printf("* ");
            ++k;
        }

        printf("\n");
    }

    return 0;
}
```

This program prompts the user to enter the number of rows for the full pyramid and then prints the pattern using asterisks (`*`). Each row has a specific number of asterisks, forming a full pyramid pattern. The spaces are used to center the pyramid.



**Polymorphism** is one of the four fundamental principles of Object-Oriented Programming (OOP), along with encapsulation, inheritance, and abstraction. Polymorphism allows objects to be treated as instances of their parent class, enabling flexibility and extensibility in software design.

There are two types of polymorphism in programming:

1. **Compile-time Polymorphism (Static Binding or Early Binding):**
   - Compile-time polymorphism is achieved through function overloading and operator overloading.
   - Function Overloading Example:
     ```cpp
     #include <iostream>
     using namespace std;

     class MathOperations {
     public:
         int add(int a, int b) {
             return a + b;
         }

         double add(double a, double b) {
             return a + b;
         }
     };

     int main() {
         MathOperations math;
         cout << "Sum of integers: " << math.add(5, 10) << endl;
         cout << "Sum of doubles: " << math.add(3.5, 2.5) << endl;
         return 0;
     }
     ```
   - In this example, the `add` function is overloaded with different parameter types, and the appropriate function is called based on the arguments during compile-time.

2. **Run-time Polymorphism (Dynamic Binding or Late Binding):**
   - Run-time polymorphism is achieved through virtual functions and is closely related to inheritance and the use of pointers/references.
   - Virtual Function Example:
     ```cpp
     #include <iostream>
     using namespace std;

     class Shape {
     public:
         virtual void draw() {
             cout << "Drawing a shape." << endl;
         }
     };

     class Circle : public Shape {
     public:
         void draw() override {
             cout << "Drawing a circle." << endl;
         }
     };

     class Square : public Shape {
     public:
         void draw() override {
             cout << "Drawing a square." << endl;
         }
     };

     int main() {
         Shape* shapePtr;

         Circle circle;
         Square square;

         shapePtr = &circle;
         shapePtr->draw();  // Output: Drawing a circle

         shapePtr = &square;
         shapePtr->draw();  // Output: Drawing a square

         return 0;
     }
     ```
   - Here, the `draw` function is declared as virtual in the base class (`Shape`). When a derived class object is accessed through a base class pointer, the appropriate overridden function is called at runtime, based on the actual object type.

Polymorphism allows for more flexibility and adaptability in software design by enabling code to work with objects of multiple types in a unified manner.
## **Lab 1: C Language Basics**

### **1. Basic Syntax**

- **`#include <stdio.h>`**: Includes the standard input/output library.

- **`main()` Function**: Program entry point, `int main() { ... }`.

- **`printf()` and `scanf()`**: Input/output functions using format specifiers for data types.

- Key Points

  :

  - Each line of code ends with a semicolon (`;`).
  - `return 0;` indicates the program executed successfully.

### **2. Data Types**

- **Integer Types**: `int`, `long`, `unsigned int`.

- **Floating Point Numbers**: `float`, `double`.

- Format Specifiers

  :

  - `%d`: Integer, `%f`: Floating-point number, `%s`: String.
  - `\n` represents a newline.

### **3. Common Operations**

- Integer Division and Type Casting

  :

  - Integer division truncates decimals. Use `(float)` for type casting.

- Arrays

  :

  - Declaration: `int numbers[10];`
  - Access elements starting from index `0`: `numbers[0] = 5;`.

### **4. Strings**

- Defined as character arrays or pointers:

  ```
  char *name = "John";
  char name[] = "John";
  ```

------

## **Lab 2: Functions, Pointers, and Structures**

### **1. Functions**

- Definition and Usage

  :

  ```
  int foo(int x) { return x + 1; }
  printf("%d", foo(5));
  ```

### **2. Pointers**

- Definition and Dereferencing

  :

  ```
  int a = 10; 
  int *p = &a; 
  printf("%d", *p);
  ```

- Common Uses

  :

  - Passing by reference, dynamic memory allocation, array manipulation.

### **3. Structures**

- **Definition**:

  - Structures combine multiple variables into a single composite data type, useful for data serialization, complex data structures (e.g., linked lists, trees).

  - Example:

    ```
    struct Point {
        int x;
        int y;
    };
    struct Point p1;
    p1.x = 10;
    p1.y = 20;
    
    struct Point p2 = {30, 40};
    ```

- **Using `typedef` for Simplified Definitions**:

  ```
  typedef struct {
      int x;
      int y;
  } Point;
  Point p = {10, 20};
  ```

- **Pointer to Structures**:

  ```
  struct Point *p_ptr = &p1;
  p_ptr->x = 15; // Equivalent to (*p_ptr).x = 15;
  p_ptr->y = 25;
  ```

------

## **Lab 3: Decision Structures**

### **1. `if` Statement**

- Checks if a condition is true:

  ```
  if (x > 0) {
      printf("Positive");
  }
  ```

### **2. `if..else` Statement**

- Executes different code blocks for true or false conditions:

  ```
  if (x % 2 == 0) {
      printf("Even");
  } else {
      printf("Odd");
  }
  ```

### **3. `if..else if..else` Statement**

- Handles multiple conditions:

  ```
  if (x < 0) {
      printf("Negative");
  } else if (x == 0) {
      printf("Zero");
  } else {
      printf("Positive");
  }
  ```

------

## **Lab 4: Loops**

### **1. `while` Loop**

- Repeats code while a condition is true:

  ```
  int i = 0;
  while (i < 10) {
      i++;
  }
  ```

### **2. `do..while` Loop**

- Executes code at least once, then checks the condition:

  ```
  int i = 0;
  do {
      i++;
  } while (i < 10);
  ```

### **3. `for` Loop**

- Includes initialization, condition check, and increment in one structure:

  ```
  for (int i = 0; i < 10; i++) {
      printf("%d", i);
  }
  ```

### **4. Loop Control Directives**

- **`break`**: Terminates the loop.
- **`continue`**: Skips the current iteration and proceeds to the next.
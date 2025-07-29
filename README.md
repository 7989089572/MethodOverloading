# Method Overloading in Java

## Theory

**Method Overloading** in Java is a feature that allows a class to have more than one method with the same name, as long as their parameter lists (number, order, or type of parameters) are different. It increases the readability of the program and is used for code reusability.

**Key Points:**
- Methods must have the same name but different parameter lists.
- Return type can be different or the same, but it alone does not constitute overloading.
- Overloading is resolved at compile time (compile-time polymorphism).

**Example Use Cases:**
- Calculating area for different shapes (area(int side), area(int length, int breadth))
- Displaying information in different formats

---

## Code Example

```java
public class OverloadExample {
    // Method with one int parameter
    void display(int a) {
        System.out.println("Arguments: " + a);
    }

    // Method with two int parameters
    void display(int a, int b) {
        System.out.println("Arguments: " + a + ", " + b);
    }

    // Method with a String parameter
    void display(String s) {
        System.out.println("Arguments: " + s);
    }

    public static void main(String[] args) {
        OverloadExample obj = new OverloadExample();
        obj.display(5);
        obj.display(5, 10);
        obj.display("Hello");
    }
}
```

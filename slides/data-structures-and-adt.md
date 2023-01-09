# Introduction to Data Structures and Abstract Data Types

**Data Structures:**

- Data structures are a way of organizing and storing data so that it can be accessed and manipulated efficiently.
- There are many data structures available to store and manipulate the data depending on the requirement.
- Common data structures include lists, stacks, queues, trees, graphs, and hash tables.
- Different data structures make certain operations more efficient than others

**Abstract Data Types(ADTs):**

- An Abstract Data Type is an abstract concept that defines a data type by its behavior (what operations can be performed on it) rather than by its implementation.
- ADTs can be implemented using different data structures, and the implementation may vary depending on the requirements of the program.
- One of the important ADTs used frequently are stacks, queues, tree, graph, the implementation of trees can be BST, AVL tree etc.

```java
//Abstract Data Type example
public interface StackADT {
    public void push(int element);
    public int pop();
    public boolean isEmpty();
    public boolean isFull();
}
```

```java
//Data Structure implementation example
public class ArrayStack implements StackADT {

    int top;
    int[] stack;
    int maxSize;

    public ArrayStack(int size) {
        maxSize = size;
        stack = new int[maxSize];
        top = -1;
    }

    public void push(int element) {
        if(!isFull()) {
            top++;
            stack[top] = element;
        } else {
            throw new RuntimeException("Stack overflow");
        }
    }

    public int pop() {
        if(!isEmpty()) {
            return stack[top--];
        } else {
            throw new RuntimeException("Stack underflow");
        }
    }

    public boolean isEmpty() {
        return top == -1;
    }

    public boolean isFull() {
        return top == maxSize - 1;
    }
}
```

Main class

```java
public class Main {
    public static void main(String[] args) {

        //Create an instance of the ArrayStack with a max size of 5
        ArrayStack stack = new ArrayStack(5);

        //Push some elements onto the stack
        stack.push(1);
        stack.push(2);
        stack.push(3);

        //Print the elements of the stack in LIFO order
        System.out.println(stack.pop()); //3
        System.out.println(stack.pop()); //2

        //Check if the stack is empty
        System.out.println(stack.isEmpty()); //false
    }
}
```

The `ArrayStack` class implements all the methods specified in the `StackADT` interface. In the main method, you create an instance of `ArrayStack` and you can push and pop elements from the stack as well as check if it's empty or not. The implementation of the StackADT is using Arrays Data Structure. In place of Array we could have used LinkedList also. The way we push, pop elements remains the same. It is just the implementation which changes.

Note that the `ArrayStack` class uses a fixed-size array to store the elements, and it will throw a runtime exception if you try to push more elements than the maximum size, or pop an element from an empty stack.

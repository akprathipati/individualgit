## Welcome to GitHub Pages


Welcome to the individualgit wiki!
## Github Link: [Review Ticket grading done by KYLE](https://github.com/gracele246/theshop/issues/2)

## Github Link: [Team](https://github.com/gracele246/theshop)
## Repel Link: [Repel for week 2](https://replit.com/@Akprathipati/AKdata#week_1/W1_C2.java)
## Repel Link: [Repel for week 3](https://replit.com/@Akprathipati/LLLLClacl#.replit)
 
DEF: linked list is a linear collection of data elements whose order is not given by their physical placement in memor
 
DEF:T> specifically stands for generic type. According to Java Docs - A generic type is a generic class or interface that is parameterized over types.

### College Board Notes
## CollegeBoard Notes: [Document](https://docs.google.com/document/d/1AIvtYBSqMLNqruzeudRC560-xHbVl7lelLFy1LClEEY/edit)
## AP Classroom FRQ: [pdf document](https://apcentral.collegeboard.org/courses/ap-computer-science-a/exam/past-exam-questions)

### Study 
- I will review all my notes and work on the practice FRQ's seen above. 
- I need to spent some time looking at the different types of data structures (like hashmaps, tuples, and arrays) and saw if they were primitive or non-primitive types.
- I need to work on datastructes and data types as well. 

### TT notes(data structures)
- matrixes
- Sort algo
Merge sort is one of the most flexible sorting algorithms in java known to mankind (yes, no kidding). It uses the divide and conquers strategy for sorting elements in an array. It is also a stable sort, meaning that it will not change the order of the original elements in an array concerning each other. The underlying strategy breaks up the array into multiple smaller segments till segments of only two elements (or one element) are obtained. Now, elements in these segments are sorted and the segments are merged to form larger segments. This process continues till the entire array is sorted.

Heap sort is one of the most important sorting methods in java that one needs to learn to get into sorting. It combines the concepts of a tree as well as sorting, properly reinforcing the use of concepts from both. A heap is a complete binary search tree where items are stored in a special order depending on the requirement. A min-heap contains the minimum element at the root, and every child of the root must be greater than the root itself. The children at the level after that must be greater than these children, and so on. Similarly, a max-heap contains the maximum element at the root. For the sorting process, the heap is stored as an array where for every parent node at the index i, the left child is at index 2 * i + 1, and the right child is at index 2 * i + 2.

## Repel Link: [Repel for Data](https://replit.com/@Akprathipati/akcode)

## Code Sniped: [Repel for Data](https://github.com/akprathipati/individualgit/blob/main/data)
## Code Sniped: [Swap Numbers](https://github.com/akprathipati/individualgit/tree/main)

 Imperative vs. Object Oriented Paradigms

Imperative Paradigms are more step-by-step than Object Oriented Paradigms. OOP relies on classes and objects, although the methods have Imperative Paradigms.

Java Arrays

public static Animal[] animalData() {
	return new Animal[]{
	        new Animal("Lion", 8, "Gold"),
	        new Animal("Pig", 3, "Pink"),
		new Animal("Robin", 7, "Red"),
		new Animal("Cat", 10, "Black"),
		new Animal("Kitty", 1, "Calico"),
		new Animal("Dog", 14, "Brown")
	};
}
Java Dictionaries

private final Map<String, Integer> OPERATORS = new HashMap<>();
    {
        // Map<"token", precedence>
        OPERATORS.put("*", 3);
        OPERATORS.put("/", 3);
        OPERATORS.put("%", 3);
        OPERATORS.put("+", 4);
        OPERATORS.put("-", 4);
    }
    
    

-A queue can be reversed by using a stack:

1. Remove all the elements from the queue and push them to a stack.
2. Pop-out all the elements from the stack and push them back to the queue.
3. The queue is revered, print the elements of the queue.

```java
public class LinkedList
{
    private Object opaqueObject;  // opaqueObject means specific type is not known, as LinkedList are not specific to a data type
    private LinkedList prevNode;
    private LinkedList nextNode;

    /**
     *  Constructs a new element with object objValue,
     *  followed by object address
     *
     * @param  opaqueObject  Address of Object
     */
    public LinkedList(Object opaqueObject, LinkedList node)
    {
        this.setObject(opaqueObject);
        this.setPrevNode(node);
        this.setNextNode(null);
    }
```

## TT2

**When using a calculator, it is difficult to calculate with precedence rules. The reverse polish notation is used because the format that the equation is in is easier for machines to interpret rather than the notation we are used to, infix notation, where the operator is in between the numbers.**

Example:

Reverse Polish Notation is a way of expressing arithmetic expressions that avoids the use of brackets to define priorities for evaluation of operators. In ordinary notation, one might write

(3 + 5) * (7 – 2)

and the brackets tell us that we have to add 3 to 5, then subtract 2 from 7, and multiply the two results together. In RPN, the numbers and operators are listed one after another, and an operator always acts on the most recent numbers in the list. The numbers can be thought of as forming a stack, like a pile of plates. The most recent number goes on the top of the stack. An operator takes the appropriate number of arguments from the top of the stack and replaces them by the result of the operation.

In this notation the above expression would be

3 5 + 7 2 – *

Reading from left to right, this is interpreted as follows:

1. Push 3 onto the stack.
2. Push 5 onto the stack. Reading from the top, the stack now contains (5, 3).
3. Apply the + operation: take the top two numbers off the stack, add them together, and put the result back on the stack. The stack now contains just the number 8.
4. Push 7 onto the stack.
5. Push 2 onto the stack. It now contains (2, 7, 8).
6. Apply the – operation: take the top two numbers off the stack, subtract the top one from the one below, and put the result back on the stack. The stack now contains (5, 8).
7. Apply the * operation: take the top two numbers off the stack, multiply them together, and put the result back on the stack. The stack now contains just the number 40, which is the mathematically correct answer.
8. How we can use a public static void main method to print the answer, 40, out.

**Below are some code snippets where the procedure is impelmented**

**Below is an example formatted constructor to implement such a calculator:**

```java
// Create a 1 argument constructor expecting a mathematical expression
    public Calculator(String expression) {
        // original input
        this.expression = expression;

        // parse expression into terms
        this.termTokenizer();

        // place terms into reverse polish notation
        this.tokensToReversePolishNotation();

        // calculate reverse polish notation
        this.rpnToResult();
    }
```
**Here is where precedence is established after operators and seperators are separated**

```java
    // Test if token is an operator
    private boolean isOperator(String token) {
        // find the token in the hash map
        return OPERATORS.containsKey(token);
    }

    // Test if token is an seperator
    private boolean isSeperator(String token) {
        // find the token in the hash map
        return SEPARATORS.containsKey(token);
    }

    // Compare precedence of operators.
    private Boolean isPrecedent(String token1, String token2) {
        // token 1 is precedent if it is greater than token 2
        return (OPERATORS.get(token1) - OPERATORS.get(token2) >= 0) ;
    }
```
Now the expression is converted into an Arraylist and implements each operator and separator in one-by-one.

```java
    // Term Tokenizer takes original expression and converts it to ArrayList of tokens
    private void termTokenizer() {
        // contains final list of tokens
        this.tokens = new ArrayList<>();

        int start = 0;  // term split starting index
        StringBuilder multiCharTerm = new StringBuilder();    // term holder
        for (int i = 0; i < this.expression.length(); i++) {
            Character c = this.expression.charAt(i);
            if ( isOperator(c.toString() ) || isSeperator(c.toString())  ) {
                // 1st check for working term and add if it exists
                if (multiCharTerm.length() > 0) {
                    tokens.add(this.expression.substring(start, i));
                }
                // Add operator or parenthesis term to list
                if (c != ' ') {
                    tokens.add(c.toString());
                }
                // Get ready for next term
                start = i + 1;
                multiCharTerm = new StringBuilder();
            } else {
                // multi character terms: numbers, functions, perhaps non-supported elements
                // Add next character to working term
                multiCharTerm.append(c);
            }

        }
        // Add last term
        if (multiCharTerm.length() > 0) {
            tokens.add(this.expression.substring(start));
        }
    }
```
**A tester method is built to print the final answer.

```java
    // Tester method
    public static void main(String[] args) {
        // Random set of test cases
        Calculator simpleMath = new Calculator("100 + 200  * 3");
        System.out.println("Simple Math\n" + simpleMath);

        System.out.println();

        Calculator parenthesisMath = new Calculator("(100 + 200)  * 3");
        System.out.println("Parenthesis Math\n" + parenthesisMath);

        System.out.println();

        Calculator fractionMath = new Calculator("100.2 - 99.3");
        System.out.println("Fraction Math\n" + fractionMath);

        System.out.println();

        Calculator moduloMath = new Calculator("300 % 200");
        System.out.println("Modulo Math\n" + moduloMath);

        System.out.println();

        Calculator divisionMath = new Calculator("300/200");
        System.out.println("Division Math\n" + divisionMath);

        System.out.println();

        Calculator multiplicationMath = new Calculator("300 * 200");
        System.out.println("Multiplication Math\n" + multiplicationMath);

        System.out.println();

        Calculator allMath = new Calculator("200 % 300 + 5 + 300 / 200 + 1 * 100");
        System.out.println("All Math\n" + allMath);

        System.out.println();

        Calculator allMath2 = new Calculator("200 % (300 + 5 + 300) / 200 + 1 * 100");
        System.out.println("All Math2\n" + allMath2);

        System.out.println();

        Calculator allMath3 = new Calculator("200%(300+5+300)/200+1*100");
        System.out.println("All Math3\n" + allMath3);

        System.out.println();

        Calculator expMath = new Calculator("8 ^ 4");
        System.out.println("Exponential Math\n" + expMath);
        
        System.out.println();

        Calculator sqrtMath = new Calculator("sqrt9");
        System.out.println("Square Root Math\n" + sqrtMath);

        System.out.println();
    }
}
```

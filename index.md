## Welcome to GitHub Pages

Mon: 

-Study/ watch videos for unit 1-3
-Go over the practice FRQ 



Tues: 

-Study unit 3-5 CB 
-Study FRQ’s from college board 
-Go over the MC 
- Do study analysis 


Wed: 

-unit 6 from CB 
-Study unit 6 frq 
-work on classes and getters and setters 
-More work on MCQ’s questions
- Watch ap live review videos 1-2



Thurs: 
- unit 7 
- FRQ unit 7 
- Watch ap live review videos 3-4


Fri:
- unit 8 & 9 
- FRQ for the units 
- Watch ap live review videos 5-6
Ajay gadacha vidoes: 
## Ajay: [Ajay video ](https://www.youtube.com/watch?v=P--N35m1X-E)
Summary: After this week, I will get a good look at my weakness: I think that FRQ's are going to be the hardest since that requires a lot more etchnical skills. I think I may do fine of the MC so far. I think the AP CB vidoes live review that they do will be helful. 





## Repel Link: [New Repel](https://replit.com/@Akprathipati/Akdatastructures?from=notifications#Sorts.java)

Sort Implementations & Big O Complexities
Sorting is when you are placing items in a list in order based on what you require. This is an algorithm that helps utilize data structures as well!  

1. Bubble Sort
Bubble sort Bubble sort works by swapping adjacent elements if they’re not in the desired order. They are compared with 2 numbers, so it isn't the most effective method.
Here is an example picture of Bubble Sort:
```java
for (int x = 0; x < array.size(); x++) {
            for (int y = 0; y < array.size() - 1; y++) {
                if (array.get(y) > array.get(y + 1)) {
                    int temporary = array.get(y);
                    array.set(y, array.get(y + 1));
                    array.set(y + 1, temporary);
                }
            }
        }
```
Basically all this code is doing is first getting our 2 variables: x and y. Each one has a certain value. In this example, we want to switch both the values. So we create a temporary which stores the values until the switch is made. 
Once the switch is done, the x and y values will switch. 
Worse time complexity of: On^2
2. Selection Sort
finds the lowest number in the list from the unsorted part and drops it at the beginning of the list. Selection sort also divides the array into a sorted and unsorted subarray
It keeps iterating through the sorted codes until it doesn’t have to do anything anymore.

https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.programiz.com%2Fdsa%2Fselection-sort&psig=AOvVaw1H7h5hUcY2P4v6dnUkZbMA&ust=1649266103619000&source=images&cd=vfe&ved=0CAoQjRxqFwoTCJCIyZS5_fYCFQAAAAAdAAAAABAD![image](https://user-images.githubusercontent.com/54961927/161815198-7b63aa1a-2a23-4264-b9ac-5b0cdac32d33.png)



It has an O(n2) time complexity, which makes it inefficient on large lists,but it seems to be much better than bubble sort. 
3. Insertion Sort
This also splits into subarrays with a sorted and unsorted part.
Here is a code snippet that looks at this:
```java
public static void insertSort(ArrayList<Integer> array) {
        int n = array.size();
        for (int i = 1; i < n; ++i) {
            int key = array.get(i);
            int j = i - 1;
            while (j >= 0 && array.get(j) > key) {
                array.set(j + 1, array.get(j));
                j = j - 1;
            }
            array.set(j + 1, key);
        }

    }
```    
 
In this code section, the code is essentially just iterating through the entire list and comparing the select number the number before it. If the number before it is smaller, then it will stay in place. It keeps looking through it’s list  until it finds a number that it is bigger than itself, and then it will switch lol. 
It does this process for each object in the code and will continue until it completely sorts itself.
takes: O ( n 2 ) O(n^2) O(n2) time. It has great efficincy. 

BIG O NOTATION
O(l) - constant time This means that the algorithm requires the same fixed number of steps regardless of the size. O(n) - linear time This means that the algorithm requires a number of steps proportional to the size of the task. If a task is more complex, then it will require more time overall. The purpose of Big O notation is to calculate the time it p(n) = aknk + ak-1nk-1 + … + a1n + a0 One way to calculate it, we can use a series method.
Constant naoiton is the best way.


## Github Link: [Review Ticket grading done by Tanmay](https://github.com/gracele246/theshop/issues/14)

## Github Link: [Team](https://github.com/gracele246/theshop)
## Repel Link: [New Repel](https://replit.com/@Akprathipati/Akdatastructures?from=notifications#Sorts.java)

 
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
Bubble sort 
Bubble sort works by swapping adjacent elements if they're not in the desired order. They are comapred with 2 numbers, so it isnt the most effectve method. 
time Complexity time complexity would be O(n^2).
Inseration Sort 
3 5 7 8 4 2 1 9 6: We take 4 and remember that that's what we need to insert. Since 8 > 4, we shift.
3 5 7 x 8 2 1 9 6: Where the value of x is not of crucial importance, since it will be overwritten immediately (either by 4 if it's its appropriate place or by 7 if we shift). Since 7 > 4, we shift.
3 5 x 7 8 2 1 9 6
3 x 5 7 8 2 1 9 6
3 4 5 7 8 2 1 9 6
O(n^2).
Selection sort 
Selection Sort also divides the array into a sorted and unsorted subarray

Merge Sort uses recursion to solve the problem of sorting more efficiently than algorithms previously presented, and in particular it uses a divide and conquer approach.
https://s3.amazonaws.com/stackabuse/media/sorting-algorithms-in-java-1.png![image](https://user-images.githubusercontent.com/54961927/161633647-546aae19-2167-485b-810d-54268edb36de.png)

BIG O NOTATION 
O(l) - constant time
This means that the algorithm requires the same fixed number of steps regardless of the size. 
O(n) - linear time
This means that the algorithm requires a number of steps proportional to the size of the task.
If a task is more complex, then it will require more time overall. 
The purpose of Big O notation is to calculate the time it 
p(n) = aknk + ak-1nk-1 + ... + a1n + a0
One way to calculate it, we can use a series method. 

Constant naoiton is the best way.





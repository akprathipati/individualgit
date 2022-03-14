## Welcome to GitHub Pages


Welcome to the individualgit wiki!


### AP Classroom
https://apcentral.collegeboard.org/courses/ap-computer-science-a/exam/past-exam-questions 

https://longbaonguyen.github.io/courses/apcsa/apjava.html 
another thing






### TT notes
- matrixes
- Order of databases

All numbers move to their respective places bit by bit, left to right, like bubbles slowly rising from a body of water.

If you'd like to read a detailed, dedicated article for Bubble Sort, we've got you covered!
Implementation

We're going to implement Bubble Sort in a similar way we've laid it out in words. Our function enters a while loop in which it goes through the entire array swapping as needed.

We assume the array is sorted, but if we're proven wrong while sorting (if a swap happens), we go through another iteration. The while-loop then keeps going until we manage to pass through the entire array without swapping:

public static void bubbleSort(int[] a) {
    boolean sorted = false;
    int temp;
    while(!sorted) {
        sorted = true;
        for (int i = 0; i < array.length - 1; i++) {
            if (a[i] > a[i+1]) {
                temp = a[i];
                a[i] = a[i+1];
                a[i+1] = temp;
                sorted = false;
            }
        }
    }
}
When using this algorithm we have to be careful how we state our swap condition.

For example, if I had used a[i] >= a[i+1] it could have ended up with an infinite loop, because for equal elements this relation would always be true, and hence always swap them.

### Database Work
 https://replit.com/@Akprathipati/pagesjava-1#src/Matrix.java 



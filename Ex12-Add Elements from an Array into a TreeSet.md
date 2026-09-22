# Ex12 Add Elements from an Array into a TreeSet
## DATE:17-09-2026
## AIM:
To write a Java program that adds elements from an array into a TreeSet and displays the elements in sorted order.
## Algorithm
1. Start the program.
2. Create an array containing a few integer elements.
3. Create a TreeSet to store the elements in sorted order.
4. Use a loop to add each element of the array into the TreeSet.
5. Display the elements of the TreeSet in sorted order.
6. Stop the program.  

## Program:
```
/*
Program that adds elements from an array into a TreeSet and displays the elements in sorted order.
Developed by: JAI HARISH R
RegisterNumber:  212224040124
*/
```

```java

import java.util.*;

public class ArrayToTreeSet {

    public static TreeSet<Integer> convertArrayToTreeSet(int[] arr) {
        List<Integer> list = new ArrayList<>();
        for(int x : arr){
            list.add(x);
        }
        
        TreeSet<Integer> treeSet = new TreeSet<>(list);
        return treeSet;
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        int[] arr = new int[n];
        for (int i = 0; i < n; i++) {
            arr[i] = sc.nextInt();
        }

        TreeSet<Integer> treeSet = convertArrayToTreeSet(arr);
        System.out.println("Elements in TreeSet:");
        for (int num : treeSet) {
            System.out.println(num);
        }

        sc.close();
    }
}

```

## Output:

<img width="773" height="541" alt="image" src="https://github.com/user-attachments/assets/77f1cf07-9b72-4508-b503-49177da08b94" />


## Result:
The program successfully adds elements from an array into a TreeSet.

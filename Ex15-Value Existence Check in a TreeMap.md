# Ex15 Value Existence Check in a TreeMap
## DATE:17-09-2026
## AIM:
To write a Java program that checks whether a given value exists in a TreeMap.

## Algorithm
1. Start the program.
2. Create a TreeMap to store key–value pairs.
3. Insert some sample key–value pairs into the TreeMap.
4. Display the contents of the TreeMap.
5. Use the containsValue() method to check whether a specific value exists in the map.
6. Display the result based on the check.
7. Stop the program.  

## Program:
```
/*
Program to checks whether a given value exists in a TreeMap.
Developed by: JAI HARISH R
RegisterNumber:  212224040124
*/
```

```java

import java.util.*;

public class TreeMapValueExistenceCheck {

    public static void checkValue(TreeMap<Integer, String> map, String searchValue) {
        if(map.containsValue(searchValue)){
            System.out.println("Value \""+searchValue+"\" exists in the TreeMap.");
        }else{
            System.out.println("Value \""+searchValue+"\" does not exist in the TreeMap.");
        }
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        TreeMap<Integer, String> map = new TreeMap<>();

        int n = sc.nextInt();

        for (int i = 0; i < n; i++) {
            int key = sc.nextInt();
            sc.nextLine();  
            String value = sc.nextLine();
            map.put(key, value);
        }
        String searchValue = sc.nextLine();

        checkValue(map, searchValue);
        sc.close();
    }
}

```

## Output:

<img width="1201" height="826" alt="image" src="https://github.com/user-attachments/assets/5c33b138-3016-4c93-8c65-a514b048f552" />



## Result:
Thus, the program successfully checks whether a specified value exists in a TreeMap using the containsValue() method.

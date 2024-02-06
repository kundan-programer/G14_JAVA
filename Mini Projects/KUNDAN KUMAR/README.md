1...........................
import java.util.Scanner;

public class sum {
  public static void main(String[] args) {
    int arr[] = { 2, 3, 8, 5, 6, 7, 1, 9, 3 };
    int sum = 0;
    int l = arr.length;
    for (int i = 0; i < l; i++) {
      sum = sum + arr[i];

    }
    System.out.println("the sum of values of array is:" + sum);
  }

}

Output: the sum of values of array is:44 

4..........................

import java.util.Scanner;

public class sum {
    public static void main(String[] args) {
        int arr[]={2,3,8,5,6,7,1,9,3};
        int avg = 0;
        int l=arr.length;
        for(int i=0;i<l;i++)
        {
            avg=avg+arr[i];

        }
        avg=avg/l;
        System.out.println("the average of values of array is "+avg);
    }
  }
Output: the average of values of array is 4
 


4.............................................
import java.util.Arrays;

public class reverse {
  public static void main(String[] args) {
    int arr[] = { 5, 47, 8, 9, 62 };
    int low = 0, high = arr.length - 1;
    int temp = 0;
    System.out.println("Original Array : " + Arrays.toString(arr));
    while (low < high) {
      temp = arr[low];
      arr[low] = arr[high];
      arr[high] = temp;
      low++;
      high--;
    }
    System.out.println("reverse is: ");
    for (int i : arr) {
      System.out.print(+i + " ");
    }
  }
}

5............................................
import java.util.Arrays;

public class dupe {
  public static void main(String[] args) {
    int[] arr = { 4, 1, 5, 2, 5, 1, 3, 6, 4, 2 };
    for (int i = 0; i < arr.length - 1; i++) {
      for (int j = i + 1; j < arr.length; j++) {
        if ((arr[i] == arr[j]) && (i != j)) {
          System.out.println("Duplicate Element : " + arr[j]);
        }
      }
    }
  }

  
 
 8.........................................


import java.util.Arrays;

public class equalarray {
  public static void main(String[] args) {
    int a[] = { 8, 5, 2 };
    int b[] = { 8, 5, 2 };
    Arrays.sort(a);
    Arrays.sort(b);

    boolean equal = true;
    int al = a.length;
    int bl = b.length;
    if (al == bl) {
      for (int i = 0; i < al; i++) {
        if (a[i] == b[i])
          continue;
        else {
          equal = false;
        }
      }
      if (equal)
        System.out.println("the arrays are equal");
      else
        System.out.println("not equal");
    }
  }

 9...................................................

import java.io.*;
import java.util.*;

public class misssing {
  public static void main(String[] args) {
    int arr[] = { 1, 3, 7, 5, 6, 2 };
    int n = arr.length;

    {
      int i;
      int temp[] = new int[n + 1];
      for (i = 0; i <= n; i++) {
        temp[i] = 0;
      }

      for (i = 0; i < n; i++) {
        temp[arr[i] - 1] = 1;
      }

      int ans = 0;
      for (i = 0; i <= n; i++) {
        if (temp[i] == 0)
          ans = i + 1;
      }
      System.out.println(ans);
    }

  }

}

10...........................
import java.util.Arrays;

public class sumequal10 {
  public static void main(String[] args) {
    int a[] = { 10, 5, 7, 20, 35 };
    int l = a.length;
    int sum = 0;
    boolean test = false;
    System.out.println("Array is" + Arrays.toString(a));
    for (int i = 0; i < l; i++) {
      if (a[i] % 10 == 0) {
        sum = sum + a[i];
      } else
        continue;

    }
    if (sum == 30)
      test = true;
    System.out.println(test);

  }
}

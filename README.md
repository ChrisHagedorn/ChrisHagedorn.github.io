# ChrisHagedorn.github.io

## Algorithms

### Find Largest Number

```java
    static int findLargestNum(int[] a) {
        int largestNumber = a[0];
        for (int i = 0; i < a.length - 1; i++) {
            if (largestNumber < a[i + 1]) {
                largestNumber = a[i + 1];
            } else {
            }
        }
        return largestNumber;
    }
```

### Bubble Sort
```java

    static void bubbleSort(int[] ar) {
        boolean changeMade = false;
        for (int i = 0; i < ar.length - 1; i++) {
            for (int x = 0; x < ar.length - 1 - i; x++) {
                if (ar[x] > ar[x + 1]) {
                    changeMade = true;
                    int temp = ar[x];
                    ar[x] = ar[x + 1];
                    ar[x + 1] = temp;
                    
                    if (!changeMade) {
                        return;
                    } else {
                        changeMade = false;

                    }
                }

            }

        }
    }
  ```
  
  ### Selection Sort
  ```java

      static void selectionSort(int[] ar) {
        for(int i = 0; i < ar.length - 1; i++){
            int minPos = getMinPos(ar, i);
            int tmp = ar[i];
            ar[i] = ar[minPos];
            ar[minPos] = tmp;
            
        
        }

    }

    private static int getMinPos(int[] ar, int start) {
        int min = ar[start];
        int minPos = start;
        for (int i = start; i < ar.length; i++) {
            if (ar[i] < min) {
                min = ar[i];
                minPos = i;

            }

        }
        return minPos;

    }
```

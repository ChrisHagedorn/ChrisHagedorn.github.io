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

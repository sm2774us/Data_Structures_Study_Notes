# Data structures and Algorithms

## Complexity (Big O)

Complexity of an algorithm measures time and memory. How long does one algorithm takes to finish? How much memory does it use?

We measure these values in terms of the input size (Usually for the input size we use the letter $n$)

We can analyze algorithms in the Best case, Average case and Worst case.

Best case measures the quickest way for an algorithm to finish.

Average case measures what time does the algorithm need to finish on average.

Worst case measures the slowest time for an algorithm to finish.

### General idea

1. Big O: ![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%20%5Clarge%20%5Cmathcal%7BO%7D%28n%5E2%29) - the algorithm takes **at most** ![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%20%5Clarge%20n%5E2) steps to finish in the **WORST CASE**.
2. Little o: ![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%20%7Bo%7D%28n%5E2%29) - the algorithm takes **less than** ![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%20%5Clarge%20n%5E2) steps to finish in the **WORST CASE**.
3. Big Omega: ![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%20%5COmega%28n%5E2%29) - the algorithm takes **at least** ![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%20%5Clarge%20n%5E2) steps to finish in the **BEST CASE**.
4. Little Omega: ![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%20%5Comega%28n%5E2%29) - the algorithm takes **more than** ![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%20%5Clarge%20n%5E2) steps to finish in the **BEST CASE**.
5. Big Theta: ![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%20%5CTheta%28n%5E2%29) - the combination of ![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%20%5Clarge%20%5Cmathcal%7BO%7D%28n%5E2%29) and ![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%20%5COmega%28n%5E2%29). Meaning the algorithm takes at least ![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%20%5Clarge%20n%5E2) steps to finish and takes at most ![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%20%5Clarge%20n%5E2) steps to finish, i.e. it always takes ![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%20%5Clarge%20n%5E2) steps.

### Comparison of orders of common functions

![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%20%5Cmathcal%7BO%7D%281%29%20%3C%20%5Cmathcal%7BO%7D%28loglog%28n%29%29%20%3C%20%5Cmathcal%7BO%7D%28log%28n%29%29%20%3C%20%5Cmathcal%7BO%7D%28log%5E2%28n%29%29%20%3C%20%5Cmathcal%7BO%7D%28%5Csqrt%7Bn%7D%29%20%3C%20%5Cmathcal%7BO%7D%28n%29%20%3C%20%5Cmathcal%7BO%7D%28nlog%28n%29%29%20%3C%20%5Cmathcal%7BO%7D%28n%5E2%29%20%3C%20%5C%5C%20%3C%20%5Cmathcal%7BO%7D%28n%5E3%29%20%3C%20%5Cmathcal%7BO%7D%282%5En%29%20%3C%20%5Cmathcal%7BO%7D%283%5En%29%20%3C%20%5Cmathcal%7BO%7D%28n%21%29%20%3C%20%5Cmathcal%7BO%7D%28n%5En%29%20%3C%20%5Cmathcal%7BO%7D%283%5E%7Bn%5E2%7D%29%20%3C%20%5Cmathcal%7BO%7D%282%5E%7Bn%5E3%7D%29)

### Big O cheat sheet

https://www.bigocheatsheet.com/

### Formal definitions

![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%20%5Cmathcal%7BO%7D%28f%28n%29%29%3D%5C%7Bg%28n%29%3A%20%5Cexists%20c%20%3E%200%2C%20%5Cexists%20n_0%20%3E%200%20%5Cmid%200%20%5Cle%20g%28n%29%20%5Cle%20cf%28n%29%20%5Cspace%20%5Cforall%20n%20%5Cge%20n_0%20%5C%7D)

![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%20%5CTheta%28f%28n%29%29%3D%5C%7Bg%28n%29%3A%20%5Cexists%20c_1%20%3E%200%2C%20%5Cexists%20c_2%20%3E%200%2C%20%5Cexists%20n_0%20%3E%200%20%5Cmid%200%20%5Cle%20c_1f%28n%29%20%5Cle%20g%28n%29%20%5Cle%20c_2%20f%28n%29%20%5Cspace%20%5Cforall%20n%20%5Cge%20n_0%20%5C%7D)

![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%20%5COmega%28f%28n%29%29%3D%5C%7Bg%28n%29%3A%20%5Cexists%20c%20%3E%200%2C%20%5Cexists%20n_0%20%3E%200%20%5Cmid%200%20%5Cle%20cf%28n%29%20%5Cle%20g%28n%29%20%5Cspace%20%5Cforall%20n%20%5Cge%20n_0%20%5C%7D)

![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%20%7Bo%7D%28f%28n%29%29%3D%5C%7Bg%28n%29%3A%20%5Cforall%20c%20%3E%200%20%5Cspace%20%5Cexists%20n_0%20%3E%200%20%5Cmid%200%20%5Cle%20g%28n%29%20%3C%20cf%28n%29%20%5Cspace%20%5Cforall%20n%20%5Cge%20n_0%20%5C%7D)

![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%20%5Comega%28f%28n%29%29%3D%5C%7Bg%28n%29%3A%20%5Cforall%20c%20%3E%200%20%5Cspace%20%5Cexists%20n_0%20%3E%200%20%5Cmid%200%20%5Cle%20cf%28n%29%20%3C%20g%28n%29%20%5Cspace%20%5Cforall%20n%20%5Cge%20n_0%20%5C%7D)

### Examples

![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%20%5Cmathcal%7BO%7D%2834n%5E4&plus;5%29%20%3D%20n%5E4)

![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%20%5Cmathcal%7BO%7D%282%5En&plus;n%5E%7B1024%7D&plus;log%28n%29%29%20%3D%202%5En)

![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%20%5Cmathcal%7BO%7D%285N%20&plus;%20%5Cfrac%7B1%7D%7B2%7D%20M%29%20%3D%20N%20&plus;%20M)

![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%20%5Cmathcal%7BO%7D%28n%5E2%29) means that if our algorithm takes input of 10 elements it will need 100 steps to finish in the worst case. If the input is of 100 elements it will need 10000 steps to finish in the worst case.

### Constants and Big O

Usually we discard constants when using Big O, but in some cases the constant can be meaningful for small input sizes. In the following example ![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%20%5Cmathcal%7BO%7D%28n%5E2%29) is faster than ![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%20%5Cmathcal%7BO%7D%28n%29) because our complexities are ![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%20n%5E2) and ![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%209n) so for ![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%20n%20%3C%209) the ![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%20n%5E2) algorithm is faster than the ![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%209n) one.

![](https://i.imgur.com/qv7rO70.png)

## Sorting

Sorting means ordering a set of elements in a sequence.

We can sort a set of elements whose elements are in partial order. Partial order is a relation with the following properties:

1. Antisymmetry - For every 2 elements in the set (A, B), if ![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%20A%20%5Cle%20B) and ![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%20B%20%5Cle%20A) then ![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%20A%3DB).
2. Transitivity - For every 3 elements in the set (A, B, C), if ![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%20A%20%5Cle%20B) and ![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%20B%20%5Cle%20C) then ![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%20A%20%5Cle%20C).
3. Reflexivity - For every element in the set A, ![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%20A%20%5Cle%20A).

### Sorting properties

#### Stable sort

A sorting algorithm is stable if two equal objects appear in the same order in the ordered output as they appeared in the unsorted input.

> Example input: ![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%201%2C%202%2C%203_a%2C%208%2C%205%2C%203_b). Here ![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%203_a) and ![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%203_b) are simply a 3 but we have marked them to follow what happens with them after the sorting.
>
> Example output: ![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%201%2C2%2C3_a%2C3_b%2C5%2C8)
>
> Unstable sort output: ![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%201%2C2%2C3_b%2C3_a%2C5%2C8)

#### In place sort

Uses only a small constant amount of extra memory. In place sort means the elements are swapped around. Out of place means we use another extra array to swap items around.

#### Number of comparisons

How many times do we need to compare 2 elements. For most sorts this represents the time complexity.

#### Adaptive sort

Determines whether the sorting algorithm runs faster for inputs that are partially or fully sorted. If an algorithm is unadaptive it runs for the same time on sorted and unsorted input. If an algorithm is adaptive it runs faster on sorted input than on unsorted input.

#### Online sort

Determines if an algorithm needs all the items from the input to start sorting. If an algorithm is online it can start sorting input that is given in parts. If an algorithm is offline it can start sorting only after it has the whole input.

#### External sort

Allows sorting data which cannot fit into memory. Such algorithms are designed to sort massive amounts of data (Gigabytes, Terabytes, etc.)

#### Parallel sort

An algorithm which can be ran on multiple threads at the same time, speeding the running time.

#### Locality

An algorithm which heavily uses the processor cache to speed up its execution. The data processed needs to be sequentially located.

### Helper code

```c++
// swap the values of two variables
void swap(int & a, int & b) {
    int tmp = a;
    a = b;
    b = tmp;
}
```

### Bubble sort

| Bubble sort           | n = input size     |
| --------------------- | ------------------ |
| Time complexity       | ![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%20%5Cmathcal%7BO%7D%28n%5E2%29) |
| Space complexity      | ![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%20%5Cmathcal%7BO%7D%281%29)   |
| Adaptive              | Yes                |
| Stable                | Yes                |
| Number of comparisons | ![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%20%5Cmathcal%7BO%7D%28n%5E2%29) |
| Number of swaps       | ![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%20%5Cmathcal%7BO%7D%28n%5E2%29) |
| Online                | No                 |
| In place              | Yes                |

Honorable mention - Cocktail shaker sort, similar to bubble and selection sort. It’s like the Online version of bubble sort.

#### Clean code

```c++
void bubbleSort(int * array, int length) {
    for (int bubbleStartIndex = 0; bubbleStartIndex < length; bubbleStartIndex++) {
        for (int bubbleMovedIndex = 0; bubbleMovedIndex < length - 1; bubbleMovedIndex++) {
            if (array[bubbleMovedIndex] > array[bubbleMovedIndex+1]) {
                swap(array[bubbleMovedIndex], array[bubbleMovedIndex+1]);
            }
        }
    }
}
```

#### Short code

```c++
void bubbleSort(int * array, int length) {
    for (int i = 0; i < length; i++) {
        for (int k = 0; k < length - 1; k++) {
            if (array[k] > array[k+1]) {
                swap(array[k], array[k+1]);
            }
        }
    }
}
```

#### Optimization 1 - make it faster

```c++
void bubbleSort(int * array, int length) {
    for (int i = 0; i < length; i++) {
        for (int k = 0; k < length - 1 - i; k++) { // length - 1 - i = 2x less iterations
            if (array[k] > array[k+1]) {
                swap(array[k], array[k+1]);
            }
        }
    }
}
```

#### Optimization 2 - make it adaptive

```c++
void bubbleSort(int * array, int length) {
    for (int i = 0; i < length; i++) {
        bool swappedAtLeastOnce = false; // add a flag to check if a swap has occurred

        for (int k = 0; k < length - 1 - i; k++) {
            if (array[k] > array[k+1]) {
                swap(array[k], array[k+1]);
                swappedAtLeastOnce = true;
            }
        }
        
        if (!swappedAtLeastOnce) { // if there were no swaps, it's ordered
            break;
        }
    }
}
```

### Selection sort

| Selection sort        | n = input size     |
| --------------------- | ------------------ |
| Time complexity       | ![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%20%5Cmathcal%7BO%7D%28n%5E2%29) |
| Space complexity      | ![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%20%5Cmathcal%7BO%7D%281%29)   |
| Adaptive              | No                 |
| Stable                | No                 |
| Number of comparisons | ![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%20%5Cmathcal%7BO%7D%28n%5E2%29) |
| Number of swaps       | ![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%20%5Cmathcal%7BO%7D%28n%29)   |
| Online                | No                 |
| In place              | Yes                |

#### Key points

1. It’s better than bubble sort in cases we need to sort items which are very large in size because it has $\mathcal{O}(n)$ swaps.

#### Clean code

```c++
void selectionSort(int * array, int length) {
    for (int currentIndex = 0; currentIndex < length; currentIndex++) {
        int smallestNumberIndex = currentIndex;

        for (int potentialSmallerNumberIndex = currentIndex + 1; 
             	potentialSmallerNumberIndex < length;
             	potentialSmallerNumberIndex++) {
            if (array[potentialSmallerNumberIndex] < array[smallestNumberIndex]) {
                smallestNumberIndex = potentialSmallerNumberIndex;
            }
        }
        
        swap(array[currentIndex], array[smallestNumberIndex]);
    }
}
```

#### Short code

```c++
void selectionSort(int * array, int length) {
    for (int i = 0; i < length; i++) {
        int index = i;

        for (int k = i + 1; k < length; k++) {
            if (array[k] < array[index]) {
                index = k;
            }
        }
        
        swap(array[i], array[index]);
    }
}
```

### Insertion sort

| Insertion sort        | n = input size     |
| --------------------- | ------------------ |
| Time complexity       | ![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%20%5Cmathcal%7BO%7D%28n%5E2%29) |
| Space complexity      | ![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%20%5Cmathcal%7BO%7D%281%29)   |
| Adaptive              | Yes                |
| Stable                | Yes                |
| Number of comparisons | ![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%20%5Cmathcal%7BO%7D%28n%5E2%29) |
| Number of swaps       | ![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%20%5Cmathcal%7BO%7D%28n%5E2%29) |
| Online                | Yes                |
| In place              | Yes                |

#### Key points

1. The best algorithm for sorting small arrays.
2. Often combined with other algorithms for optimal runtime.

#### Clean code

```c++
void insertionSort(int * array, int length) {
    for (int nextItemToSortIndex = 1; nextItemToSortIndex < length; nextItemToSortIndex++) {
        for (int potentiallyBiggerItemIndex = nextItemToSortIndex; 
             	potentiallyBiggerItemIndex > 0 && 
             	array[potentiallyBiggerItemIndex] < array[potentiallyBiggerItemIndex - 1];
             	potentiallyBiggerItemIndex--) {
            swap(array[potentiallyBiggerItemIndex], array[potentiallyBiggerItemIndex-1]);
        }
    }
}
```

#### Short code

```c++
void insertionSort(int * array, int length) {
    for (int i = 1; i < length; i++) {
        for (int k = i; k > 0 && array[k] < array[k - 1]; k--) {
            swap(array[k], array[k-1]);
        }
    }
}
```

### Merge sort

| Merge sort            | n = input size          |
| --------------------- | ----------------------- |
| Time complexity       | ![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%20%5Cmathcal%7BO%7D%28n*log%28n%29%29) |
| Space complexity      | ![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%20%5Cmathcal%7BO%7D%28n%29) |
| Adaptive              | No                      |
| Stable                | Yes                     |
| Number of comparisons | ![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%20%5Cmathcal%7BO%7D%28n*log%28n%29%29) |
| External              | Yes                     |
| Parallel              | Yes                     |
| Online                | No                      |
| In place              | No                      |

#### Key points

1. Every array of 0 or 1 elements is sorted.
2. Merging requires additional memory.
3. Splitting the array in 2 every time gives us $log(n)$ levels.
4. On each level we have $\mathcal{O}(n)$ for the merging operation.

Honorable mention - Ford–Johnson aka. Merge-insertion sort. Cool idea, but not practical enough.

Important algorithm: Timsort - Absolute beast with ![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%20%5Cmathcal%7BO%7D%28nlogn%29) worst case and ![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%20%5Cmathcal%7BO%7D%28n%29) best case. Implementation can be found here: https://github.com/tvanslyke/timsort-cpp

![](https://i.imgur.com/obZrU8h.png)

#### Clean code

```c++
void merge(int * originalArray, int * mergeArray, int start, int mid, int end) {
    int leftIndex = start;
    int rightIndex = mid + 1;
    int sortedIndex = start;

    while (leftIndex <= mid && rightIndex <= end) {
        if (originalArray[leftIndex] <= originalArray[rightIndex]) {
            mergeArray[sortedIndex] = originalArray[leftIndex];
            leftIndex++;
        } else {
            mergeArray[sortedIndex] = originalArray[rightIndex];
            rightIndex++;
        }

        sortedIndex++;
    }

    while (leftIndex <= mid) {
        mergeArray[sortedIndex] = originalArray[leftIndex];
        leftIndex++;
        sortedIndex++;
    }
    while (rightIndex <= end) {
        mergeArray[sortedIndex] = originalArray[rightIndex];
        rightIndex++;
        sortedIndex++;
    }

    for (int i = start; i <= end; i++) {
        originalArray[i] = mergeArray[i];
    }
}

void mergeSortRecursive(int * original, int * mergeArray, int start, int end) {
    if (start < end) {
        int mid = (start + end) / 2;

        mergeSortRecursive(original, mergeArray, start, mid);
        mergeSortRecursive(original, mergeArray, mid + 1, end);

        merge(original, mergeArray, start, mid, end);
    }
}

void mergeSort(int * array, int length) {
    int * mergeArray = new int[length];
    mergeSortRecursive(array, mergeArray, 0, length - 1);
    delete[] mergeArray;
}
```

#### Short code

```c++
void merge(int * originalArray, int * mergeArray, int start, int mid, int end) {
    int left = start;
    int right = mid + 1;

    for (int i = start; i <= end; i++) {
        if (left <= mid && (right > end || originalArray[left] <= originalArray[right])) {
            mergeArray[i] = originalArray[left];
            left++;
        } else {
            mergeArray[i] = originalArray[right];
            right++;
        }
    }

    for (int i = start; i <= end; i++) {
        originalArray[i] = mergeArray[i];
    }
}

void mergeSortRecursive(int * originalArray, int * mergeArray, int start, int end) {
    if (start < end) {
        int mid = (start + end) / 2;

        mergeSortRecursive(originalArray, mergeArray, start, mid);
        mergeSortRecursive(originalArray, mergeArray, mid + 1, end);

        merge(originalArray, mergeArray, start, mid, end);
    }
}

void mergeSort(int * array, int length) {
    int * mergeArray = new int[length];
    mergeSortRecursive(array, mergeArray, 0, length - 1);
    delete[] mergeArray;
}
```

### Quick sort

| Quick sort                     | n = input size                        |
| ------------------------------ | ------------------------------------- |
| Time complexity (Worst case)   | ![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%20%5Cmathcal%7BO%7D%28n%5E2%29)                    |
| Time complexity (Average case) | ![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%20%5Cmathcal%7BO%7D%28n*log%28n%29%29)               |
| Space complexity               | ![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%20%5Cmathcal%7BO%7D%28log%28n%29%29)                 |
| Adaptive                       | No                                    |
| Anti-Adaptive                  | Yes (the more randomness, the better) |
| Stable                         | No                                    |
| Number of comparisons          | ![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%20%5Cmathcal%7BO%7D%28n*log%28n%29%29)               |
| Parallel                       | Yes                                   |
| Online                         | No                                    |
| In place                       | Yes                                   |
| Locality                       | Yes                                   |

#### Key points

1. Quick sort adores chaos. That’s why a common strategy is to shuffle the array before sorting it.

C++ STL sorting algorithm is Introsort, which is a hybrid between quicksort and heapsort.

Quick sort optimization for arrays with many equal numbers - three-way partitioning, aka Dutch national flag.

Quick sort can also be optimized with picking 2 pivots instead of 1 - multi-pivot quicksort.

#### Why is quick sort usually faster than merge sort and other fast algorithms?

The table bellow is an approximation of the time required to access data from the disk/ram/CPU cache. It gives us an idea why quick sort is indeed quick. Quick sort being in-place gets reduced to problems in the CPU cache very fast. Merge sort on the other hand uses additional memory, so it has 2 arrays it works with essentially. Often these 2 arrays cannot simultaneously enter the cache so they have to be read from RAM, which is very slow. Quick sort, however, uses only one array which gets pulled into the CPU cache and operations on it are very fast.

| Memory hierarchy | CPU cycles | size   |
| ---------------- | ---------- | ------ |
| HDD              | 500, 000   | 1 TB   |
| RAM              | 100        | 4 GB   |
| L2 cache         | 10         | 512 kb |
| L1 cache         | 1          | 32 kb  |

#### Uses apart from sorting

1. Find k-th biggest/smallest element

#### Clean code using Lomuto partitioning

```c++
int partition(int * array, int startIndex, int endIndex) {
    int pivot = array[endIndex];
    int pivotIndex = startIndex;

    for (int i = startIndex; i <= endIndex; i++) {
        if (array[i] < pivot) {
            swap(array[i], array[pivotIndex]);
            pivotIndex++;
        }
    }

    swap(array[endIndex], array[pivotIndex]);
    return pivotIndex;
}

void _quickSort(int * array, int startIndex, int endIndex) {
    if (startIndex < endIndex) {
        int pivot = partition(array, startIndex, endIndex);
        _quickSort(array, startIndex, pivot - 1);
        _quickSort(array, pivot + 1, endIndex);
    }
}

void quickSort(int * array, int length) {
    _quickSort(array, 0, length - 1);
}
```

#### Short code using Lomuto partitioning

```c++
int partition(int * array, int start, int end) {
    int pivot = array[end];
    int pivotIndex = start;
    for (int i = start; i <= end; i++) {
        if (array[i] < pivot) {
            swap(array[i], array[pivotIndex]);
            pivotIndex++;
        }
    }
    swap(array[end], array[pivotIndex]);
    return pivotIndex;
}

void _quickSort(int * array, int start, int end) {
    if (start < end) {
        int pivot = partition(array, start, end);
        _quickSort(array, start, pivot - 1);
        _quickSort(array, pivot + 1, end);
    }
}

void quickSort(int * array, int length) {
    _quickSort(array, 0, length - 1);
}
```

#### Optimization 1 - pivot is random number

```c++
#include <random>
int generateRandomNumber(int from, int to) {
    std::random_device dev;
    std::mt19937 rng(dev());
    std::uniform_int_distribution<std::mt19937::result_type> dist6(from,to);

    return dist6(rng);
}

int partition(int * array, int start, int end) {
    int randomIndex = generateRandomNumber(start, end);
    swap(array[end], array[randomIndex]);
    
    int pivot = array[end];
    int pivotIndex = start;
    for (int i = start; i <= end; i++) {
        if (array[i] < pivot) {
            swap(array[i], array[pivotIndex]);
            pivotIndex++;
        }
    }
    swap(array[end], array[pivotIndex]);
    return pivotIndex;
}

void _quickSort(int * array, int start, int end) {
    if (start < end) {
        int pivot = partition(array, start, end);
        _quickSort(array, start, pivot - 1);
        _quickSort(array, pivot + 1, end);
    }
}

void quickSort(int * array, int length) {
    _quickSort(array, 0, length - 1);
}
```

#### Optimization 2 - shuffle before picking pivot

```c++
#include <random>
int generateRandomNumber(int from, int to) {
    std::random_device dev;
    std::mt19937 rng(dev());
    std::uniform_int_distribution<std::mt19937::result_type> dist6(from,to);

    return dist6(rng);
}

void shuffle(int * arr, int length) {
    for (int i = 0; i < length - 1; i++) {
        int swapCurrentWith = generateRandomNumber(i, length - 1);
        swap(arr[i], arr[swapCurrentWith]);
    }
}

int partition(int * array, int start, int end) {
    shuffle(array + start, end - start);

    int pivot = array[end];
    int pivotIndex = start;
    for (int i = start; i <= end; i++) {
        if (array[i] < pivot) {
            swap(array[i], array[pivotIndex]);
            pivotIndex++;
        }
    }
    swap(array[end], array[pivotIndex]);
    return pivotIndex;
}

void _quickSort(int * array, int start, int end) {
    if (start < end) {
        int pivot = partition(array, start, end);
        _quickSort(array, start, pivot - 1);
        _quickSort(array, pivot + 1, end);
    }
}

void quickSort(int * array, int length) {
    _quickSort(array, 0, length - 1);
}
```

#### Short code using Hoare partitioning

```c++
int partition(int * array, int start, int end)  {
    int pivot = array[(start + end) / 2];
    int left = start - 1;
    int right = end + 1;

    while (true) {
        do {
            left++;
        } while (array[left] < pivot);

        do {
            right--;
        } while (array[right] > pivot);

        if (left >= right) {
            return right;
        }

        swap(array[left], array[right]);
    }
}

void _quickSort(int * array, int start, int end) {
    if (start < end) {
        int pivot = partition(array, start, end);
        _quickSort(array, start, pivot - 1);
        _quickSort(array, pivot + 1, end);
    }
}

void quickSort(int * array, int length) {
    _quickSort(array, 0, length - 1);
}
```

### Counting sort

| Counting sort                | n = input size, k = max number |
| ---------------------------- | ------------------------------ |
| Time complexity (Worst case) | ![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%20%5Cmathcal%7BO%7D%28n%20&plus;%20k%29)           |
| Time complexity (Best case)  | ![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%20%5Cmathcal%7BO%7D%28n%29)               |
| Space complexity             | ![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%20%5Cmathcal%7BO%7D%28k%29)               |

#### Key points

1. Not a comparison sort.
2. Very efficient for an array of integers with many repeating integers with small difference between the biggest and smallest integer.

#### Uses apart from sorting

1. Counting inversions

#### Counting sort for positive numbers

```c++
void countingSort(int * array, int length) {
    int maxNumber = 0;
    for (int i = 0; i < length; i++) {
        if (array[i] > maxNumber) {
            maxNumber = array[i];
        }
    }

    int * countingArray = new int[maxNumber + 1];
    for (int i = 0; i < maxNumber + 1; i++) {
        countingArray[i] = 0;
    }

    for (int i = 0; i < length; i++) {
        countingArray[array[i]]++;
    }

    int sortedIndex = 0;
    for (int i = 0; i < length; i++) {
        while (countingArray[sortedIndex] == 0) {
            sortedIndex++;
        }

        array[i] = sortedIndex;
        countingArray[sortedIndex]--;
    }

    delete[] countingArray;
}
```

### Bucket sort

| Bucket sort                    | n = input size, k = number of buckets |
| ------------------------------ | ------------------------------------- |
| Time complexity (Worst case)   | ![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%20%5Cmathcal%7BO%7D%28n%5E2%29)                    |
| Time complexity (Average case) | ![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%20%5Cmathcal%7BO%7D%28n&plus;%5Cfrac%7Bn%5E2%7D%7Bk%7D&plus;k%29)      |
| Space complexity               | ![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%20%5Cmathcal%7BO%7D%28nk%29)                     |

#### Key points

1. It’s a distribution sort, not a comparison sort.
2. Very situational sort.
3. The bellow code is a sample implementation for floats between 0 and 1.

#### Code

```c++
#include <iostream>
#include <vector>
#include <algorithm>
void bucketSort(double *array, int length) {
    std::vector<double> buckets[length];

    for(int i = 0; i < length; i++) {
        buckets[int(length * array[i])].push_back(array[i]);
    }

    for(int i = 0; i < length; i++) {
        sort(buckets[i].begin(), buckets[i].end());
    }

    int index = 0;
    for(int i = 0; i < length; i++) {
        while(!buckets[i].empty()) {
            array[index] = buckets[i][0];
            index++;
            buckets[i].erase(buckets[i].begin());
        }
    }
}
```

### Radix sort

### Radix sort

| Radix sort                     | n = input size                   |
| ------------------------------ | -------------------------------- |
| Time complexity (Worst case)   | ![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%20%5Cmathcal%7BO%7D%28n%5E2%29)               |
| Time complexity (Average case) | ![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%20%5Cmathcal%7BO%7D%28n&plus;%5Cfrac%7Bn%5E2%7D%7Bk%7D&plus;k%29) |
| Space complexity               | ![equation](https://latex.codecogs.com/svg.latex?%5Cbg_white%20%5Cmathcal%7BO%7D%28nk%29)                |

#### Key points

1. Good on multi-threaded machines.

#### Code

```c++
#include <iostream>
#include <cmath>
#include <list>

int abs(int a) {
    return a >= 0 ? a : -a;
}

void radixSort(int * array, int length) {
    int maxNumber = 0;
    for (int i = 0; i < length; i++) {
        if (abs(array[i]) > maxNumber) {
            maxNumber = abs(array[i]);
        }
    }

    int maxDigits = log10(maxNumber) + 1;

    std::list<int> pocket[10];

    for(int i = 0; i < maxDigits; i++) {
        int m = pow(10, i + 1);
        int p = pow(10, i);

        for(int j = 0; j < length; j++) {
            int temp = array[j] % m;
            int index = temp / p;
            pocket[index].push_back(array[j]);
        }

        int count = 0;
        for(int j = 0; j<10; j++) {
            while(!pocket[j].empty()) {
                array[count] = *(pocket[j].begin());
                pocket[j].erase(pocket[j].begin());
                count++;
            }
        }
    }
}
```

# Selection-sort

# Pseudocode
## FindMinIndex:

    FindMinIndex(Arr[], start, end)    
        min_index = start    
        
        FOR i from (start + 1) to end:    
            IF Arr[i] < Arr[min_index]:    
                min_index = i    
            END of IF    
        END of FOR    
      Return min_index

Suppose, there are ‘n’ elements in the array. Therefore, at worst case, there can be n iterations in FindMinIndex() for start = 1 and end = n. We did not take any auxiliary space.

Therefore,

# Time complexity: O(n)

# Space complexity: O(1)

# Selection Sort:

    SelectionSort(Arr[], arr_size):    
        FOR i from 1 to arr_size:    
            min_index = FindMinIndex(Arr, i, arr_size)    
        
            IF i != min_index:    
                swap(Arr[i], Arr[min_index])    
            END of IF    
        END of FOR

Suppose, there are ‘n’ elements in the array. Therefore, at worst case, there can be n iterations in FindMinIndex() for start = 1 and end = n. No auxiliary space used.

Total iterations = (n – 1) + (n – 2) + . . . + 1 = (n * (n – 1)) / 2 = (n2 – n) / 2

Therefore,

# Time complexity: O(n2)

# Space complexity: O(1)

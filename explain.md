First loop:
It copies elements from index 0 up to but not including smallest_index from arr to temporary
So since smallest index is at 1 it copies index 0 to temporary
Essential is preserves the part of the arr before the smallest_index

Second loop:
Starts from element after smallest_index and shifts everything one step to the left into temporary
It places arr[i] into temporary[i - 1]
It skips smallest_index (removing it)
The i -1 effectively closes the gap left by removing element

Walk through:
If arr = [10,-5,11,2]
First loop takes arr[0] and assigns it to temporary[0]
Second loop takes arr[2,3] and assigns it to temporary[1,2]
So temporary is now [10,11,2]
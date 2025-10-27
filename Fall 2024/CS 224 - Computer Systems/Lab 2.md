```
function bubble-sort(A : list of numbers)
  n = number of numbers in A
  repeat
    swapped = false
    for i := 0 to n - 2
      if A[i] > A[i + 1] then
        swap A[i] with A[i + 1]
        swapped = true
      end if
    end for
  until not swapped
end function
```

```c
void bubble-sort(int * arr) {
	int n = sizeof(arr) / sizeof(arr[0]);

	for (int i = 0; i < n - 2; i++) {
		if (arr[i] > arr[i + 1]) {
			
		}
	}
}
```
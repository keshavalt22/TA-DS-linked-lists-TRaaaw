## Implement Sorting Algorithms

We learned about different sorting algorithms in the previous block. Implement the sorting algorithms you learned in the videos as a function.

1. Write down the steps to perform for different sorting algorithms i.e bubble, insertion and selection. Write in your own words. After writing the algorithm take an example of an array and draw the diagram for each step for different algorithm.

Example:

#### Bubble Sort

step-1: We will compare the first item with the second. If the first item is bigger than the second item we will swap them so that the bigger one stays in the second position.

step-2: And then compare second with third item. If second item is bigger than the third, we swap them. otherwise, they stayed in their position. Hence, the biggest among first three is in the third position.

step-3: We keep doing it. Until we hit the last element of the array. In that way we bubble up the biggest item of the array to the right most position of the array.

step-4: Now we will repeat the step 1, 2 and 3 but we will keep in mind not to touch the last element.

![Bubble Sort Example](./bubble.png)

<!-- You answer -->

2. Create a function named `bubbleSort` that accepts an array of numbers and returns the array with sorted values. The elements should be in ascending order. Use the bubble sorting algorithms. After writing the function test it with an array and check if you are getting the right output.

```js
function bubbleSort(arr) {
  let n = arr.length;
  for(let i = 0; i < n; i++){
    for(let j = 0; j< n - i - 1; j++){
      if(arr[j] > arr[j + 1]){
        [arr[j], arr[j + 1]] = [arr[j+1], arr[j]]
      }
    }
  }
  console.log(arr)
}
```

3. Create a function named `selectionSort` that accepts an array of numbers and returns the array with sorted values. The elements should be in ascending order. Use the selection sorting algorithms. After writing the function test it with an array and check if you are getting the right output.

```js
function selectionSort() {
  let n = arr.length, key, j;
  for(let i = 1; i < n; i++){
    key = arr[i];
    j = i - 1;
    while(j >= 0&& arr[j] >= key){
      arr[j + 1] = arr[j];
      j = j - 1;
    }
    arr[j1+ 1] = key;
  }
  console.log(arr);
}
```

4. Create a function named `insertionSort` that accepts an array of numbers and returns the array with sorted values. The elements should be in ascending order. Use the insertion sorting algorithms. After writing the function test it with an array and check if you are getting the right output.

```js
function insertionSort() {
  // your code
}
```

5. After writing all the sorting algorithm check the output with the array given below and make sure you are getting the right output.

```js
let values = [76, 34, 12, 32, 4, 2, 123, 5667, 8, 1, 3];
```

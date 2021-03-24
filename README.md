# Data Structures and Algorithms



### Big O Analysis

For each of the following functions:
- Specify the time complexity.
- Briefly explain your answer.



---
Function 1 Time Complexity:

Function 1 Explanation: 
```
function bobIsFirst(people){
  return people[0] == 'bob'
}
```
---
Function 2 Time Complexity:

Function 2 Explanation: 
```
function wordOccurrence(word, phrase){
  let result = 0
  const array = phrase.split(' ')
  for(let i = 0; i < array.length; i++){
    if(word.toLowerCase() === array[i].toLowerCase()){
      result++;
    }
  }
  return result
}
```
---
Function 3 Time Complexity:

Function 3 Explanation: 
```
function sort(list){
  for(let i = 0; i < list.length - 1; i++){
    for(let j  = 0; j < list.length - 2; j++){
      if(list[j+1] < list[j]){
        const temp = list[j];
        list[j] = list[j+1];
        list[j+1] = temp;
      }
    }
  }
  return list;
}
```

---

### Written Questions

- What method would you use to look up a word in a dictionary?

- Imagine you have a closet full of shirts. What can you do to organize your shirts for easy retrieval?

- Describe advantages and disadvantages of the most popular sorting algorithms.

---

### HackerRank Problems

- [Diagonal Difference](https://www.hackerrank.com/challenges/diagonal-difference/problem) (Algorithm, Warmup)
- [Left Rotation](https://www.hackerrank.com/challenges/array-left-rotation/problem) (Data Structures, Array)
- [Get Node Value](ckerrank.com/challenges/get-the-value-of-the-node-at-a-specific-position-from-the-tail/) (Data Structures, Linked List)
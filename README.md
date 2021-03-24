# Data Structures and Algorithms

1. Fork and clone this repo
2. Fill out the Big O and Written Questions in this README.
3. Complete the HackerRank challenges on hackerrank.com
4. You have 1 hour and 20 minutes


### Big O Analysis

---
Function 1 Time Complexity:

O(1)

Explain your answer:
this only makes one comparison and only runs once
```
function bobIsFirst(people){
  return people[0] == 'bob'
}
```
---
Function 2 Time Complexity:
O(n)
Explain your answer:
It will always run a set amount of times given the input size (n)
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
O(n^2)
Explain your answer:
for each element(n) iterated, it runs a second loop iterating through 'n' elements. n^2

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

- What method would you use to look up a word in a dictionary (book, not Python)?

- Imagine you have a closet full of shirts. What can you do to organize your shirts for easy retrieval?
  -You can organize the shirts based different occasions such as casual, professinal, night-out, etc..

- Describe advantages and disadvantages of the most popular sorting algorithms.
 - many of the best algorithms (ex:merge sort) work better with larger sets of data 
   due their constant or O(log(n)) time complexities
                        
---

### HackerRank Problems

- [Diagonal Difference](https://www.hackerrank.com/challenges/diagonal-difference/problem) (Algorithm, Warmup)
- [Left Rotation](https://www.hackerrank.com/challenges/array-left-rotation/problem) (Data Structures, Array)
- [Get Node Value](https://www.hackerrank.com/challenges/get-the-value-of-the-node-at-a-specific-position-from-the-tail) (Data Structures, Linked List)

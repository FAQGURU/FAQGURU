## Code Problems

[Test divisors of three](#test-divisors-of-three)

[Sum of Array Plus One](#sum-of-array-plus-one)

[String Rotation](#string-rotation)

[Oddball sum](#oddball-sum)

[Simple clock angle](#simple-clock-angle)

[Sum of several arrays](#sum-of-several-arrays)

[Lucky sevens](#lucky-sevens)

[Two sum problem](#two-sum-problem)

[Implement a queue using a linked list](#implement-a-queue-using-a-linked-list)

[Tree Level Order Print](#tree-level-order-print)

[Stock maximum profit](#stock-maximum-profit)

[Find Word Positions in Text](#find-word-positions-in-text)

[Determine overlapping numbers in ranges](#determine-overlapping-numbers-in-ranges)

[Throttle Function Implementation](#throttle-function-implementation)

[Dutch national flag sorting problem](#dutch-national-flag-sorting-problem)

[Step-by-step solution for step counting using recursion](#step-by-step-solution-for-step-counting-using-recursion)

[Implement Bubble Sort](#implement-bubble-sort)

[Implement a queue using two stacks](#implement-a-queue-using-two-stacks)

[Implement pow(a,b) without multiplication or division](#implement-powab-without-multiplication-or-division)

[Generate all balanced bracket combinations](#generate-all-balanced-bracket-combinations)

[All Permutations (Anagrams) of a String](#all-permutations-anagrams-of-a-string)

[Merge two sorted linked lists](#merge-two-sorted-linked-lists)

[Insert an interval into a list of sorted disjoint intervals](#insert-an-interval-into-a-list-of-sorted-disjoint-intervals)

[Find all string combinations consisting only of 0, 1 and ?](#find-all-string-combinations-consisting-only-of-0-1-and-)

[Quickly calculate the cube root of 6 digit numbers](#quickly-calculate-the-cube-root-of-6-digit-numbers)

[Transform Word](#transform-word)

[Find the missing value in a set of number from 1 to n](#missing-value-set-of-numbers-1-to-n)


### Test divisors of three

We'll solve this problem by first creating a loop that will print each number from low to high. Once we have the code for that written, we'll add a conditional that will check if the number is evenly divisible by 3 by using the mod operator.

```js
function test_divisors(low, high) {
  
  // we'll store all numbers and strings within an array
  // instead of printing directly to the console
  var output = [];
  
  for (var i = low; i <= high; i++) {
    
    // simply store the current number in the output array
    output.push(i);
    
    // check if the current number is evenly divisible by 3
    if (i % 3 === 0) { output.push('div3'); }
    
  }
  
  // return all numbers and strings
  return output;
  
}

test_divisors(2, 10);
```

###### Source

* https://coderbyte.com/algorithm/test-divisors-of-three

[[↑] Back to top](#Code%20Problems)
### Sum of Array Plus One

```js
// ES5 method is nice and clean
exports.es5 = function (array) {
  return array.reduce(function (memo, num) {
    return memo + num;
  }, array.length);
};

// Without array.reduce method isn't much different
exports.iterative = function (array) {
  var result = array.length;

  for (var i = 0; i < array.length; i++) {
    result += array[i];
  }

  return result;
};
```

###### Source

* https://github.com/blakeembrey/code-problems/tree/master/problems/sum-of-array-plus-one

[[↑] Back to top](#Code%20Problems)
### String Rotation

First make sure `a` and `b` are of the same length. Then check to see if `b` is a substring of `a` concatenated with `a`:

```js
module.exports = function (a, b) {
  return a.length === b.length && (a + a).indexOf(b) > -1;
};
```



###### Source

* https://github.com/blakeembrey/code-problems/tree/master/problems/string-rotation

[[↑] Back to top](#Code%20Problems)
### Oddball sum

To solve this challenge we'll simply loop through the array while maintaining a final count, and every time an odd number is encountered we'll add it to the count.

Without `reduce`:
```js
function oddball_sum(nums) {
 
  // final count of all odd numbers added up
  var final_count = 0;
  
  // loop through entire list
  for (var i = 0; i < nums.length; i++) {
    
    // we divide by 2, and if there is a remainder then
    // the number must be odd so we add it to final_count
    if (nums[i] % 2 === 1) {
      final_count += nums[i]
    }
    
  }
  
  return final_count;
  
}

oddball_sum([1, 2, 3, 4, 5]); 
```

With `reduce`:

```js
function oddball_sum(nums) {
  return nums.reduce(function(total, item){
  	if (item % 2 === 1) {
  		return total += item;
  	}
  	return total;
  });
}
```

###### Source

* http://prepwork.appacademy.io/coding-test-1/practice-coding-exercise/ 

[[↑] Back to top](#Code%20Problems)
### Simple clock angle

If the input is `15` then your program should return `90` because a `90`-degree angle is formed by the minute hand and the `12` o'clock mark on the clock. We'll solve this challenge by first calculating what angle is created by each minute passing on a clock. Once we calculate this number, we multiply it by the input to determine the final angle. 

A method to solve such problems is to consider the rate of change of the angle in degrees per minute. The hour hand of a normal `12-hour` analogue clock turns `360°` in `12` hours (`720` minutes) or `0.5°` per minute. The minute hand rotates through `360°` in `60` minutes or `6°` per minute.

```js
function simpleClockAngle(num) {

  // we got 6 because 360/60 = 6
  // 360 represents the full number of a degrees in a circle and
  // 60 is the number of minutes on a clock, so dividing these two numbers
  // gives us the number of degrees for one minute
  return 6 * num;

}

simpleClockAngle(15);
```



###### Source

* https://coderbyte.com/algorithm/stock-maximum-profit

[[↑] Back to top](#Code%20Problems)
### Sum of several arrays

We will solve this challenge by looping through the entire array, and then looping through each inner array adding up all the numbers.

```js
function sum_array(arr) {
  // store our final answer
  var sum = 0;
  // loop through entire array
  for (var i = 0; i < arr.length; i++) {
    // loop through each inner array
    for (var j = 0; j < arr[i].length; j++) {
      // add this number to the current final sum
      sum += arr[i][j];
    }
  }
  
  return sum;
}

sum_array([[3, 2], [1], [4, 12]]);
```

With `reduce`:

```js
function sumArray(arr) {
  return arr.reduce((t, e) => t.concat(e)).reduce((t, e) => t + e)
}
```

###### Source

* https://coderbyte.com/algorithm/sum-of-several-arrays

[[↑] Back to top](#Code%20Problems)
### Lucky sevens

To solve this challenge we'll simply loop through the array starting at the 3rd position, and checking if the number at this index plus the two previous elements sums to 7. We continue doing this as we loop through the entire array. Once we find three elements that sum to 7, we simply return `true`. If we reach the end of the array without finding elements that sum to 7, we return `false`.

```js
function lucky_sevens(arr) {
  
  // if less than 3 elements then this challenge is not possible
  if (arr.length < 3) {
    return "not possible";
  }
  
  // because we know there are at least 3 elements we can
  // start the loop at the 3rd element in the array (i=2)
  // and check it along with the two previous elements (i-1) and (i-2)
  for (var i = 2; i < arr.length; i++) {
    if (arr[i] + arr[i-1] + arr[i-2] === 7) {
      return true; 
    }
  }
  
  // if loop is finished and no elements summed to 7
  return false;
  
}

lucky_sevens([2, 1, 5, 1, 0]);
``` 



###### Source

* https://coderbyte.com/algorithm/lucky-sevens

[[↑] Back to top](#Code%20Problems)
### Two sum problem

The algorithm below makes use of hash tables which have a constant lookup time. As we pass through each element in the array, we check to see if S minus the current element exists in the hash table. We only need to loop through the array once, resulting in a running time of `O(n)` since each lookup and insertion in a hash table is `O(1)`.

```js
// our two sum function which will return
// all pairs in the array that sum up to S
function twoSum(arr, S) {

  var sums = [];
  var hashTable = {};

  // check each element in array
  for (var i = 0; i < arr.length; i++) {
 
    // calculate S - current element
    var sumMinusElement = S - arr[i];

    // check if this number exists in hash table
    // if so then we found a pair of numbers that sum to S
    if (hashTable[sumMinusElement.toString()] !== undefined) { 
      sums.push([arr[i], sumMinusElement]);
    }

    // add the current number to the hash table
    hashTable[arr[i].toString()] = arr[i];

  }

  // return all pairs of integers that sum to S
  return sums;

}

twoSum([3, 5, 2, -4, 8, 11], 7);
```



###### Source

* https://coderbyte.com/algorithm/two-sum-problem

[[↑] Back to top](#Code%20Problems)
### Implement a queue using a linked list

We will store a reference to the front and back of the queue in order to make enqueuing and dequeuing run in `O(1)` constant time. Every time we want to insert into the queue, we add the new element to the end of the linked list and update the back pointer. When we want to dequeue we return the first node in the linked list and update the front pointer.

```js
// queue is initially empty
var Queue = {front: null, back: null};

// we will use a node to keep track of the elements
// in the queue which is represented by a linked list
function Node(data, next) {
  this.data = data;
  this.next = next;
} 

// add elements to queue in O(1) time
function Enqueue(element) {
  var N = new Node(element, null);
  if (Queue.back === null) {
    Queue.front = N;
    Queue.back = N; 
  } else { 
    Queue.back.next = N; 
    Queue.back = Queue.back.next;
  } 
}

// remove first element from queue in O(1) time
function Dequeue() {
  if (Queue.front !== null) { 
    var first = Queue.front;
    Queue.front = Queue.front.next; 
    return first.data;
  } else {
    if (Queue.back !== null) { Queue.back = null; }
    return 'Cannot dequeue because queue is empty';
  }
}

Enqueue('a'); 
Enqueue('b'); 
Enqueue('c'); 
Dequeue();
```

###### Source

* https://coderbyte.com/algorithm/implement-a-queue-using-linked-list

[[↑] Back to top](#Code%20Problems)
### Tree Level Order Print

```js
module.exports = function (root) {
  // Doing a breadth first search using recursion.
  (function walkLevel (children) {
    // Create a new queue for the next level.
    var queue = [],
        output;

    // Use the map function to easily join all the nodes together while pushing
    // it's children into the next level queue.
    output = children.map(function (node) {
      // Assuming the node has children stored in an array.
      queue = queue.concat(node.children || []);
      return node.value;
    }).join(' ');

    // Log the output at each level.
    console.log(output);

    // If the queue has values in it, recurse to the next level and walk
    // along it.
    queue.length && walkLevel(queue);
  })([root]);
};
```


###### Source

* http://www.ardendertat.com/2011/12/05/programming-interview-questions-20-tree-level-order-print/

[[↑] Back to top](#Code%20Problems)
### Stock maximum profit

We'll solve the challenge the following way:

1. Iterate through each number in the list.
2. At the ith index, get the `i+1` index price and check if it is larger than the ith index price.
3. If so, set `buy_price = i` and `sell_price = i+1`. Then calculate the profit: `sell_price - buy_price`.
4. If a stock price is found that is cheaper than the current `buy_price`, set this to be the new buying price and continue from step 2.
5. Otherwise, continue changing only the `sell_price` and keep `buy_price` set.

This algorithm runs in linear time, making only one pass through the array, so the running time in the worst case is `O(n)`.

```js
function StockPicker(arr) { 
  
  var max_profit = -1;
  var buy_price = 0;
  var sell_price = 0;
  
  // this allows our loop to keep iterating the buying
  // price until a cheap stock price is found
  var change_buy_index = true;
  
  // loop through list of stock prices once
  for (var i = 0; i < arr.length-1; i++) {
    
    // selling price is the next element in list
    sell_price = arr[i+1]; 
    
    // if we have not found a suitable cheap buying price yet
    // we set the buying price equal to the current element
    if (change_buy_index) { buy_price = arr[i]; }
    
    // if the selling price is less than the buying price
    // we know we cannot make a profit so we continue to the 
    // next element in the list which will be the new buying price
    if (sell_price < buy_price) {
      change_buy_index = true; 
      continue;
    }
    
    // if the selling price is greater than the buying price
    // we check to see if these two indices give us a better 
    // profit then what we currently have
    else { 
      var temp_profit = sell_price - buy_price;
      if (temp_profit > max_profit) { max_profit = temp_profit; }
      change_buy_index = false;
    }
    
  }
  
  return max_profit;
         
}

StockPicker([44, 30, 24, 32, 35, 30, 40, 38, 15]);  
```

###### Source

* https://coderbyte.com/algorithm/stock-maximum-profit

[[↑] Back to top](#Code%20Problems)
### Find Word Positions in Text

Since we’ll have to answer multiple queries, precomputation would be useful. We’ll build a data structure that stores the positions of all the words in the text file. This is known as inverted index.

```js
module.exports = function (text) {
  var trie   = {},
      pos    = 0,
      active = trie; // Start the active structure as the root trie structure

  // Suffix a space after the text to make life easier
  text += ' ';

  // Loop through the input text adding it to the trie structure
  for (var i = 0; i < text.length; i++) {
    // When the character is a space, restart
    if (text[i] === ' ') {
      // If the current active doesn't equal the root, set the position
      if (active !== trie) {
        (active.positions = active.positions || []).push(pos);
      }
      // Reset the positions and the active part of the data structure
      pos    = i;
      active = trie;
      continue;
    }

    // Set the next character in the structure up
    active[text[i]] = (active[text[i]] || {});
    active = active[text[i]];
  }

  // Return a function that accepts a word and looks it up in the trie structure
  return function (word) {
    var i      = -1,
        active = trie;

    while (word[++i]) {
      if (!active[word[i]]) { return []; }
      active = active[word[i]];
    }

    return active.positions;
  };
};
```

###### Source

* https://github.com/blakeembrey/code-problems/tree/master/problems/word-positions

[[↑] Back to top](#Code%20Problems)
### Determine overlapping numbers in ranges

With loop:
```js
function OverlappingRanges(arr) {

  // keep a count of how many numbers overlap
  var counter = 0;
  
  // loop through one of the ranges
  for (var i = arr[0]; i < arr[1]; i++) {

    // check if a number within the first range exists
    // in the second range
    if (i >= arr[2] && i <= arr[3]) { 
      counter += 1;
    }

  }
 
  // check if the numbers that overlap is equal to or greater
  // than the last number in the array
  return (counter >= arr[4]) ? true : false;
}

OverlappingRanges([4, 10, 2, 6, 3]); 
```

Without loop:

```js
function overlapping(input){
  var nums1 = listOfNums(input[0], input[1]);
  var nums2 = listOfNums(input[2], input[3]);
  var overlappingNum = 0;

  if(nums1[0] >= nums2[0] && nums1[0] <= nums2[1]){
    overlappingNum =  nums2[1] - nums1[0] + 1;
  } else {
    overlappingNum =  nums1[1] - nums2[0] + 1;
  }
  if(overlappingNum >= input[4]){
    return true;
  }
}

function listOfNums(a, b){
  var start = a;
  var end = b;
  if(a > b){
    start = b;
    end = a;
  }

  return [a, b];
}

var a = [4, 10, 2, 6, 3];
overlapping(a)
```


###### Source

* https://coderbyte.com/algorithm/stock-maximum-profit

[[↑] Back to top](#Code%20Problems)
### Throttle Function Implementation

```js
module.exports = function (fn, delay, execAsap) {
  var timeout; // Keeps a reference to the timeout inside the returned function

  return function () {
    // Continue to pass through the function execution context and arguments
    var that = this,
        args = arguments;

    // If there is no timeout variable set, proceed to create a new timeout
    if (!timeout) {
      execAsap && fn.apply(that, args);

      timeout = setTimeout(function () {
        execAsap || fn.apply(that, args);
        // Remove the old timeout variable so the function can run again
        timeout = null;
      }, delay || 100);
    }
  };
};
```


###### Source

* https://github.com/blakeembrey/code-problems/tree/master/problems/throttle

[[↑] Back to top](#Code%20Problems)
### Dutch national flag sorting problem

The solution to this algorithm will require 3 pointers to iterate throughout the array, swapping the necessary elements.

1. Create a low pointer at the beginning of the array and a high pointer at the end of the array.
2. Create a mid pointer that starts at the beginning of the array and iterates through each element.
3. If the element at `arr[mid]` is a `2`, then swap `arr[mid]` and `arr[high]` and decrease the high pointer by `1`.
4. If the element at `arr[mid]` is a `0`, then swap `arr[mid]` and `arr[low]` and increase the low and mid pointers by `1`.
5. If the element at `arr[mid]` is a `1`, don't swap anything and just increase the mid pointer by `1`.

```js
function swap(arr, i1, i2) {
  var temp = arr[i1];
  arr[i1] = arr[i2];
  arr[i2] = temp;
}

function dutchNatFlag(arr) {
  
  var low = 0;
  var mid = 0;
  var high = arr.length - 1;
  
  // one pass through the array swapping
  // the necessary elements in place
  while (mid <= high) {
    if      (arr[mid] === 0) { swap(arr, low++, mid++); }
    else if (arr[mid] === 2) { swap(arr, mid, high--); }
    else if (arr[mid] === 1) { mid++; }
  }
  
  return arr;
  
}

dutchNatFlag([2,2,2,0,0,0,1,1]); 
```

###### Source

* https://coderbyte.com/algorithm/dutch-national-flag-sorting-problem

[[↑] Back to top](#Code%20Problems)
### Step-by-step solution for step counting using recursion

The solution to this problem requires recursion, which means to solve for a particular `N`, we need the solutions for previous N's. The solution for N steps is equal to the solutions for `N - 1` steps plus `N - 2` steps.

```js
function countSteps(N) {
  
  // just as in our solution explanation above, we know that to climb 1 step
  // there is only 1 solution, and for 2 steps there are 2 solutions
  if (N === 1) { return 1; }
  if (N === 2) { return 2; }
  
  // for all N > 2, we add the previous (N - 1) + (N - 2) steps to get
  // an answer recursively
  return countSteps(N - 1) + countSteps(N - 2);
  
}

// the solution for N = 6 will recursively be solved by calculating
// the solution for N = 5, N = 4, N = 3, and N = 2 which we know is 2
countSteps(6); 
```


###### Source

* https://coderbyte.com/algorithm/step-by-step-solution-step-walking-using-recursion

[[↑] Back to top](#Code%20Problems)
### Implement Bubble Sort

The steps in the bubble sort algorithm are:

1. Loop through the whole array starting from index `1`
2. If the number in the array at index `i-1` is greater than i, swap the numbers and continue
3. Once the end of the array is reached, start looping again from the beginning
4. Once no more elements can be swapped, the sorting is complete

```js
function swap(arr, i1, i2) {
  var temp = arr[i1];
  arr[i1] = arr[i2];
  arr[i2] = temp;
}

function bubblesort(arr) {
  
  var swapped = true;
  
  // keep going unless no elements can be swapped anymore
  while (swapped) {
    
    // set swapped to false so that the loop stops
    // unless two element are actually swapped
    swapped = false;

    // loop through the whole array swapping adjacent elements
    for (var i = 1; i < arr.length; i++) {
      if (arr[i-1] > arr[i]) {
        swap(arr, i-1, i);
        swapped = true;
      }
    }
    
  }
  
  return arr;
         
}

bubblesort([103, 45, 2, 1, 97, -4, 67]); 
```

###### Source

* https://coderbyte.com/algorithm/implement-bubble-sort

[[↑] Back to top](#Code%20Problems)
### Implement a queue using two stacks

Suppose we push `a`, `b`, `c` to a stack. If we are trying to implement a queue and we call the dequeue method 3 times, we actually want the elements to come out in the order: `a`, `b`, `c`, which is in the opposite order they would come out if we popped from the stack. So, basically, we need to access the elements in the reverse order that they exist in the stack. 

*Algorithm* for queue using two stacks:

1. When calling the enqueue method, simply push the elements into the stack 1.
2. If the dequeue method is called, push all the elements from stack 1 into stack 2, which reverses the order of the elements. Now pop from stack 2.

The worst case running time for implementing these operations using stacks is `O(n)` because you need to transfer n elements from stack 1 to stack 2 when a dequeue method is called. Pushing to stack 1 is simply `O(1)`.

```js
// implement stacks using plain arrays with push and pop functions
var Stack1 = [];
var Stack2 = [];

// implement enqueue method by using only stacks
// and the push and pop functions
function Enqueue(element) {
  Stack1.push(element);
}

// implement dequeue method by pushing all elements
// from stack 1 into stack 2, which reverses the order
// and then popping from stack 2
function Dequeue() {
  if (Stack2.length === 0) {
    if (Stack1.length === 0) { return 'Cannot dequeue because queue is empty'; }
    while (Stack1.length > 0) {
      var p = Stack1.pop();
      Stack2.push(p);
    }
  }
  return Stack2.pop();
}

Enqueue('a');
Enqueue('b');
Enqueue('c');
Dequeue(); 
```

###### Source

* https://coderbyte.com/algorithm/implement-queue-using-two-stacks

[[↑] Back to top](#Code%20Problems)
### Implement pow(a,b) without multiplication or division

The algorithm to implement:
1. Create a variable named answer
2. Loop from `1` to `n`
3. Each time through the loop we add `a` + `a` + ... (we add a to itself a times) and store result in answer
4. Then each time through the loop we perform step 3 replacing a with answer.

```js
// our modified pow function that raises a to the power of b
// without using multiplication or division
function modPow(a, n) {
  
  // convert a to positive number
  var answer = Math.abs(a);
  
  // store exponent for later use
  var exp = n;
  
  // loop n times
  while (n > 1) {
    
    // add the previous added number n times
    // e.g. 4^3 = 4 * 4 * 4
    //      4*4 = 4 + 4 + 4 + 4 = 16
    //     16*4 = 16 + 16 + 16 + 16 = 64
    var added = 0;
    for (var i = 0; i < Math.abs(a); i++) { added += answer; }
    answer = added;
    n--;
    
  }
  
  // if a was negative determine if the answer will be
  // positive or negative based on the original exponent
  // e.g. pow(-4, 3) = (-4)^3 = -64
  return (a < 0 && exp % 2 === 1) ? -answer : answer;
  
}

modPow(2, 10); 
//modPow(5, 4); 
//modPow(-4, 7); 
```

Using recursion and closures:

```js
function pow(num, e) {
  let exponent;
  let value = num;
  addup();

  function addup(outernum = num, iterate = 1) {
    if (iterate == e) {
      return;
    }
    for (let counter = 1; counter < num; counter++) {
      value += outernum;
    }
    exponent = value;
    return addup(value, iterate + 1);
  }
  return exponent;
}
```

###### Source

* https://coderbyte.com/algorithm/implement-pow-a-b-without-multiplication-division

[[↑] Back to top](#Code%20Problems)
### Generate all balanced bracket combinations

We will implement a recursive function to solve this challenge. The idea is:
1. Add a left bracket to a newly created string.
2. If a left bracket was added, potentially add a new left bracket and add a right bracket.
3. After each of these steps we add the string to an array that stores all bracket combinations.

```js
var all = [];

function parens(left, right, str) {
  
  // if no more brackets can be added then add the final balanced string
  if (left === 0 && right === 0) {
    all.push(str);
  }
  
  // if we have a left bracket left we add it
  if (left > 0) {
    parens(left-1, right+1, str+"(");
  }
  
  // if we have a right bracket left we add it
  if (right > 0) {
    parens(left, right-1, str+")"); 
  }
  
}

// the parameters parens(x, y, z) specify:
// x: left brackets to start adding
// y: right brackets we can add only after adding a left bracket
// z: the string so far
parens(3, 0, "");
console.log(all); 
```

###### Source

* https://coderbyte.com/algorithm/generate-balanced-bracket-combinations

[[↑] Back to top](#Code%20Problems)
### All Permutations (Anagrams) of a String

Remove the first character and recurse to get all permutations of length `N-1`, then insert that first character into `N-1` length strings and obtain all permutations of length `N`. The complexity is `O(N!)` because there are `N!` possible permutations of a string with length `N`, so it’s optimal.

```js
module.exports = function (string) {
  var result = {};

  // Using an immediately invoked named function for recursion.
  (function makeWord (word, remaining) {
    // If there are no more remaining characters, break and set to true
    // in the result object.
    if (!remaining) { return result[word] = true; }

    // Loop through all the remaining letters and recurse slicing the character
    // out of the remaining stack and into the solution word.
    for (var i = 0; i < remaining.length; i++) {
      makeWord(
        word + remaining[i],
        remaining.substr(0, i) + remaining.substr(i + 1)
      );
    }
  })('', string);

  // Using the ES5 Object.keys to grab the all the keys as an array.
  return Object.keys(result);
};
```

###### Source

* https://github.com/blakeembrey/code-problems/tree/master/problems/string-rotation

[[↑] Back to top](#Code%20Problems)
### Merge two sorted linked lists

Algorithm:
1. Create a new head pointer to an empty linked list.
2. Check the first value of both linked lists.
3. Whichever node from `L1` or `L2` is smaller, append it to the new list and move the pointer to the next node.
4. Continue this process until you reach the end of a linked list.

```js
function Node(data, next) {
  this.data = data;
  this.next = next;
} 

function merge(L1, L2) {
  
  // create new linked list pointer
  var L3 = new Node(null, null);
  var prev = L3;
  
  // while both linked lists are not empty
  while (L1 !== null && L2 !== null) {
    if (L1.data <= L2.data) { 
      prev.next = L1;
      L1 = L1.next;
    } else {
      prev.next = L2;
      L2 = L2.next;
    }
    prev = prev.next;
  }
  
  // once we reach end of a linked list, append the other 
  // list because we know it is already sorted
  if (L1 === null) { prev.next = L2; }
  if (L2 === null) { prev.next = L1; }
  
  // return the sorted linked list
  return L3.next;
  
}

// create first linked list: 1 -> 3 -> 10
var n3 = new Node(10, null);
var n2 = new Node(3, n3);
var n1 = new Node(1, n2);
var L1 = n1; 

// create second linked list: 5 -> 6 -> 9
var n6 = new Node(9, null);
var n5 = new Node(6, n6);
var n4 = new Node(5, n5);
var L2 = n4; 

merge(L1, L2); 
```

###### Source

* https://coderbyte.com/algorithm/merge-two-sorted-linked-lists

[[↑] Back to top](#Code%20Problems)
### Insert an interval into a list of sorted disjoint intervals

Algorithm:
1. Create an array where the final intervals will be stored.
2. Push all the intervals into this array that come before the new interval you are adding.
3. Once we reach an interval in that comes after the new interval, add our new interval to the final array.
4. From this point, check each remaining element in the array and determine if the intervals need to be merged.

```js
function insertInterval(arr, interval) {
  
  var newSet = [];
  var endSet = [];
  var i = 0;

  // add intervals that come before the new interval
  while (i < arr.length && arr[i][1] < interval[0]) {
    newSet.push(arr[i]);
    i++;
  }

  // add our new interval to this final list
  newSet.push(interval);

  // check each interval that comes after the new interval to determine if we can merge
  // if no merges are required then populate a list of the remaining intervals
  while (i < arr.length) {
    var last = newSet[newSet.length - 1];
    if (arr[i][0] < last[1]) {
      var newInterval = [Math.min.apply(null, [last[0], arr[i][0]]), Math.max.apply(null, [last[1], arr[i][1]])];
      newSet[newSet.length - 1] = newInterval;
    } else {
      endSet.push(arr[i]);
    }
    i++;
  }

  return newSet.concat(endSet);
  
}

insertInterval([[1,5],[10,15],[20,25]], [12,27]); 
```

###### Source

* https://coderbyte.com/algorithm/insert-interval-into-list-of-sorted-disjoint-intervals

[[↑] Back to top](#Code%20Problems)
### Find all string combinations consisting only of 0, 1 and ?

The general algorithm we will write a solution for is:
1. Call the function with the string and an empty set where we begin pushing `0` and `1`'s.
2. Once we reach a `?` make a copy of each string set, and for half append a `0` and for the other half append a `1`.
3. Recursively call the function with a smaller string until the string is empty.

```js
function patterns(str, all) {
  
  // if the string is empty, return all the string sets
  if (str.length === 0) { return all; }
  
  // if character is 0 or 1 then add the character to each
  // string set we currently have so far
  if (str[0] === '0' || str[0] === '1') {
    for (var i = 0; i < all.length; i++) {
      all[i].push(str[0]);  
    }
  }
  
  // for a wildcard, we make a copy of each string set
  // and for half of them we append a 0 to the string 
  // and for the other half we append a 1 to the string
  if (str[0] === '?') {
    var len = all.length;
    for (var i = 0; i < len; i++) {
      var temp = all[i].slice(0);
      all.push(temp);
    }
    for (var i = 0; i < all.length; i++) {
      (i < all.length/2) ? all[i].push('0') : all[i].push('1');  
    }
  }
  
  // recursively calculate all string sets
  return patterns(str.substring(1), all);
  
}

patterns('10?1?', [[]]);
```


###### Source

* https://coderbyte.com/algorithm/find-all-string-combinations-consisting-zero-one-wildcard

[[↑] Back to top](#Code%20Problems)
### Quickly calculate the cube root of 6 digit numbers

The general algorithm is as follows:
1. Store the first 10 cube roots, their cubes, and the last digit in the number.

 ```js
var cubes_10 = {
      '0': 0,
      '1': 1,
      '8': 8,
     '27': 7,
     '64': 4,
    '125': 5,
    '216': 6,
    '343': 3,
    '512': 2,
    '729': 9
  };
```
2. Ignore the last 3 digits of the input number, and for the remaining numbers, find the cube in the table that is less than or equal to the remaining number, and take the corresponding cube root to be the first number in your answer. 
3. For the last 3 digits that you previously ignored, loop through the table and when you get to the ith index, where i equals the last digit of the remaining 3 numbers, take the corresponding number in the right column as your answer.
4. These numbers combined are the cube root answer.

```js
function fastCubeRoot(num) {
  
  var cubes_10 = {
      '0': 0,
      '1': 1,
      '8': 8,
     '27': 7,
     '64': 4,
    '125': 5,
    '216': 6,
    '343': 3,
    '512': 2,
    '729': 9
  };
  
  // get last 3 numbers and the remaining numbers
  var arr = num.toString().split('');
  var last = arr.slice(-3);
  var first = parseInt(arr.slice(0, -3).join(''));
  
  // answer will be stored here
  var lastDigit = 0, firstDigit = 0, index = 0;
  
  // get last digit of cube root
  for (var i in cubes_10) {
    if (index === parseInt(last[last.length-1])) { lastDigit = cubes_10[i]; }
    index++;
  }
  
  // get first digit of cube root
  index = 0;
  for (var i in cubes_10) {
    if (parseInt(i) <= first) { firstDigit = index; }
    index++;
  }
  
  // return cube root answer
  return firstDigit + '' + lastDigit;
  
}

fastCubeRoot(830584);
```

###### Source

* https://coderbyte.com/algorithm/quickly-calculate-cube-root-6-digit-numbers

[[↑] Back to top](#Code%20Problems)
### Transform Word

```js
module.exports = function (dictionary, start, end) {
  // Create a function that will return an object which represents a graph
  // structure.
  var createGraph = function (dictionary) {
    var graph = {};

    // Create a simple helper function that will return a boolean whether the
    // words are one character apart
    var isOneCharDifference = function (word1, word2) {
      // If the second word is larger than the first word, reverse the
      // arguments and run again.
      if (word2.length > word1.length) {
        return isOneCharDifference(word2, word1);
      }

      // If the difference in length between the words is greater than one,
      // or the words are identical anyway, it's impossible.
      if (word1 === word2 || word2.length < word1.length - 1) {
        return false;
      }

      for (var i = 0; i < word1.length; i++) {
        // First we check whether replacing the character with the equivelent
        // from the second word with make the second word.
        if (word1.substr(0, i) + word2[i] + word1.substr(i + 1) === word2) {
          return true;
        }

        // Next we check if removing a single letter from the first word will
        // result in the second word.
        if (word1.substr(0, i) + word1.substr(i + 1) === word2) {
          return true;
        }
      }

      return false;
    };

    dictionary.forEach(function (word) {
      // Add the word to the graph structure with an array for the connecting
      // nodes.
      graph[word] = [];

      // Check all the other words in the graph so far and see if they are
      // connections.
      Object.keys(graph).forEach(function (connection) {
        if (isOneCharDifference(word, connection)) {
          graph[word].push(connection);
          // Push the word into the connection if it's been created.
          graph[connection] && graph[connection].push(word);
        }
      });
    });

    return graph;
  };

  // Find the solution.
  var graph = createGraph(dictionary);
  var shortestRoute;

  (function findRoute (word, route) {
    // If the word doesn't exist in the graph or we have gone to the word
    // before, break early.
    if (!graph[word] || ~route.indexOf(word)) { return; }

    // If the route is longer than a previous route, stop trying to loop around.
    if (shortestRoute && route.length >= shortestRoute.length) { return; }

    // Push the word into the current route
    route.push(word);

    // If the word now matches the final word, set it as the route.
    if (word === end) {
      return shortestRoute = route;
    }

    graph[word].forEach(function (connection) {
      return findRoute(connection, route.slice());
    });
  })(start, []);

  return shortestRoute;
};
```

###### Source

* https://github.com/blakeembrey/code-problems/tree/master/problems/throttle

[[↑] Back to top](#Code%20Problems)

### Find the missing value in a set of number from 1 to n

You are given a list of n-1 integers and these integers are in the range of 1 to n. There are no duplicates in list. One of the integers is missing in the list. Write an efficient code to find the missing integer.

METHOD 1(Use sum formula)
Algorithm:

1. Get the sum of numbers 
       total = n*(n+1)/2
2  Subtract all the numbers from sum and
   you will get the missing number.

Time Complexity : O(n)
   
```js
  // Function to find missing number
  function getMissingNo (a, n)
{
  var i, total;
  total  = (n+1)*(n+2)/2;
  for ( i = 0; i< n; i++)
  total -= a[i];
  return total;
}

 getMissingNo([1,2,4,5,6],5);
 
```

METHOD 2(Use XOR)

  1) XOR all the array elements, let the result of XOR be X1.
  2) XOR all numbers from 1 to n, let XOR be X2.
  3) XOR of X1 and X2 gives the missing number.
 
Time Complexity : O(n) 
 
```js

  function getMissingNo (a, n)
  {
    var x1 = a[0];
    var x2 = 1;

    /* For xor of all the elements
       in array */
    for (var i = 1; i < n; i++)
    x1 = x1 ^ a[i];

    /* For xor of all the elements
       from 1 to n+1 */
    for (var i = 2; i <= n+1; i++)
    x2 = x2 ^ i;

    return (x1 ^ x2);
  }
  
  var array = [1, 2, 4, 6, 3, 7, 8];
  getMissingNo(array,array.length);
 
```

###### Source

* https://www.geeksforgeeks.org/find-the-missing-number/

[[↑] Back to top](#Code%20Problems)

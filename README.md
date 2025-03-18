# first-demo
This is my first repository.
<br>
Author -- Vishakha Rathore.




// ASSIGNMENT - 1

// question 1--Write a program to reverse the elements of an array without using any built-in reverse functions. Your program should iterate through the array and reverse its elements in place (without creating a new array). The output should be the array with its elements in reverse order
let arr = [1, 2, 3, 4, 5];

let reversedarr=[]
for (let i = arr.length - 1; i >= 0; i--) {
    reversedarr.push(arr[i]); 
}
console.log(reversedarr);

// question -- 2-Write a program to take an array of integers as input and calculate the sum of even numbers and the sum of odd numbers separately. Your program should iterate through the array and add the even numbers to one sum and the odd numbers to another sum. Finally, print both sums.

let arr = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
let evenSum = 0;
let oddSum = 0;

for (let i = 0; i < arr.length; i++) {
    if (arr[i] % 2 === 0) {
        evenSum += arr[i];  
    } else {
        oddSum += arr[i];   
    }
}
let totalSum = evenSum + oddSum;
console.log("Sum of even arr: " + evenSum);
console.log("Sum of odd arr: " + oddSum);
console.log("Total sum (even + odd): " + totalSum);


// ASSIGNMENT - 2

// question 1--Write a JavaScript code calculateElectricityBill(units) that takes the number of electricity units consumed as input and calculates the total bill based on the following slab rates:

function calculateElectricityBill(units) {
  let billAmount = 0;
  if (units <= 100) {
    billAmount = units * 3;
  } else if (units <= 200) {
    billAmount = 100 * 3 + (units - 100) * 5;
  } else if (units <= 300) {
    billAmount = 100 * 3 + 100 * 5 + (units - 200) * 7;
  } else {
    billAmount = 100 * 3 + 100 * 5 + 100 * 7 + (units - 300) * 10;
  }

  // Apply 10% surcharge if bill exceeds ₹1000
  if (billAmount > 1000) {
    billAmount += billAmount * 0.10; 
  }

  return billAmount;
}

// Example usage:
let unitsConsumed = 350;
let totalBill = calculateElectricityBill(unitsConsumed);
console.log("Total Electricity Bill: ₹" + totalBill);

// question 2--The objective of this assignment is to help students understand and analyze the time complexity of different loop structures and nested iterations in C++. Students will calculate the time complexity for different scenarios and provide justifications for their answers.

Task 1: Basic Loop Analysis
Code:
for(int i = 0; i < n; i++) {
    cout << "PhysicsWallah\n";
}

Time Complexity Analysis:

The loop runs from i = 0 to i < n, meaning it executes n times.
Each iteration prints "PhysicsWallah", which is a constant-time operation (O(1)).
 the overall time complexity is determined by the number of iterations.

Conclusion:
The time complexity is O(n), as the loop runs n times.

Task 2: Loop with Increment of 2
Code:

for(int i = 0; i < n; i+=2) {
    cout << "PhysicsWallah\n";
}
Time Complexity Analysis:

The loop runs from i = 0 to i < n, but i is incremented by 2 after each iteration (i += 2).
This means the loop will run  n/2 times (if n is even, exactly n/2 times; if odd, it will be (n+1)/2 times).

Conclusion:
The time complexity is O(n)


Task 3: Traversing Two Arrays Separately
Code:
int a[n], b[m];
for(int i = 0; i < n; i++) {
    a[i] = i;
}
for(int i = 0; i < m; i++) {
    b[i] = m - i;
}
Time Complexity Analysis:

The first loop iterates over array a of size n 
The second loop iterates over array b of size m


Task 4: Nested Loop for Two Arrays
Code:


for(int i = 0; i < n; i++) {
    for(int j = 0; j < m; j++) {
        cout << "okay";
    }
}
Time Complexity Analysis:

The outer loop runs n times, 
the inner loop runs m times, 

Conclusion:
The time complexity is O(n * m).


Task 5: Logarithmic Complexity
Code:


int c = 0;
for(int i = 1; i < n; i *= k) {
    c++;
}








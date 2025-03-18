# first-demo
this is my first repository.
<br>
Author -- Vishakha Rathore.
// question no - 1 of assignment
let arr = [1, 2, 3, 4, 5];
let reversedarr=[]
for (let i = arr.length - 1; i >= 0; i--) {
    reversedarr.push(arr[i]); 
}
console.log(reversedarr);

// question no - 2
let numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
let evenSum = 0;
let oddSum = 0;

for (let i = 0; i < numbers.length; i++) {
    if (numbers[i] % 2 === 0) {
        evenSum += numbers[i];  
    } else {
        oddSum += numbers[i];   
    }
}
let totalSum = evenSum + oddSum;
console.log("Sum of even numbers: " + evenSum);
console.log("Sum of odd numbers: " + oddSum);
console.log("Total sum (even + odd): " + totalSum);







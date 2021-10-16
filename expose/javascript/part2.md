# Expose - Javascript Part 2

1. console.log(i) outputs the last value of i which is 3, because the for loop increments i until it's no longer less than prices.length.  The final value of i will be the first time it fails the condition. 
2. console.log(discountedPrice) outputs the last value of discountedPrice which is 150, because the last value of prices[i] is 150 and multiplying it by (1 - discount) = 150.
3. console.log(finalPrice) outputs the last value of finalPrice which is 150, because it takes the (discountedPrice * 100) / 100 to remove any floating point trailing digits and returns 150. 
4. The function will return discounted, an array of the 3 finalPrice values [50, 100, 150]  
5. ReferenceError: i is not defined.  Declaring i with let only allows it to be accessed in the for loop block.
6. ReferenceError: discountedPrice is not defined.  Declaring discountedPrice with let only allows it to be accessed in the for loop block.
7. console.log(finalPrice) outputs 150 because finalPrice is within the same scope of the main function block.  
8. The function will return discounted, an array of the 3 finalPrice values [50, 100, 150]
9. ReferenceError: i is not defined.  Declaring i with let only allows it to be accessed in the for loop block.
10. console.log(length) outputs 3, which is the length of the input prices array.
11. The function will return discounted, an array of the 3 finalPrice values [50, 100, 150].  The const array is still mutable with pushes, it just can't be re-assigned.  
12. Object accession  
    1. student['name']
    2. student['Grad Year'] 
    3. student.greeting()
    4. student['Favorite Teacher']['name']
    5. student['courseLoad'][0]
13. Arithmetic
    1.  '32', 2 was mapped to '2' then concatenated to '3'.
    2.  1, '3' was mapped to the integer 3 then 2 was subtracted from it.
    3.  3, null gets mapped to 0.
    4.  '3null', null gets mapped to 'null' then concatenated to '3'
    5.  4, true gets mapped to 1 then added to 3.
    6.  0, false gets mapped to 0 and null gets mapped to 0, added together is 0.
    7.  '3undefined', undefined gets mapped to 'undefined' and concatenated to '3'. 
    8.  NaN, '3' gets mapped to 3 and undefined gets mapped to NaN, and any numeric operation with NaN is NaN. 
14. Comparison
    1.  true, '2' gets mapped to 2 which is larger than 1
    2.  false, '2' is greater than '12' alphanumerically 
    3.  true, '2' becomes a 2 which is equivalent to 2
    4.  false, strict equality returns false because they are different types
    5.  false, true gets mapped to 1 which is not equivalent to 2
    6.  true, Boolean(2) is equivalent to true which is strictly equivalent to true
15. Non-strict equality is checked with == where type conversion occurs to determine if values are equivalent.
    Strict equality is checked with === where there is no type conversion and values must be the same type and equivalent.
16. 
for (const [key, value] of Object.entries(statistics)) {
    if (key[0] == 'r' || value % 2 == 1 ) {
        console.log(value);
    }
}
17. The result will be [ 2, 4, 6 ], the for loop iterates through the input array, calling doSomething on each element to double the value, and pushing them to newArr.
18. 
function printTime() {
    let d = new Date();
    let time = d.toLocaleTimeString();
    console.log(time);
}

var intervalID = setInterval(printTime, 1000);
19. 
1 
4 
3 
2

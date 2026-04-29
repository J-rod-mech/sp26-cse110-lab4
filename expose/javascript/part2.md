1. Line 12 prints 3 because i was declared using var, allowing access outside the local scope. The loop logic caused it to stop once i = 3, the length of the input list prices.

2. Line 13 prints 150 because discountedPrice was declared using var, allowing access outside the local scope. The last price value used was 300, which multiplied by 0.5 equals 150.

3. Line 14 prints 150 because finalPrice was declared using var, so it is accessible from any scope. Besides, console.log(finalPrice) is called in the same scope as finalPrice. finalPrice rounds the last discountedPrice, 150, to the nearest hundredths place: 150.

4. The function returns the list [50, 100, 150]. The loop logic iterates through the prices, then multiplies it by the discount factor (in this case 1 - 0.5 = 0.5), adding it to the new discounted list. Going from [100, 200, 300] returns [50, 100, 150].

5. Line 12 throws a ReferenceError: i is not defined because i was declared using let inside the for loop, and this line attempts to access i outside the scope of the loop.

6. Line 13 throws a ReferenceError: discountedPrice is not defined because discountedPrice was declared using let inside the for loop, and this line attempts to access discountedPrice outside the scope of the loop.

7. Line 14 prints 150 because while finalPrice was declared using let, this was done so outside the for loop, which is also where console.log(finalPrice) is being called. finalPrice rounds the last discountedPrice, 150, to the nearest hundredths place: 150.

8. The function returns the list [50, 100, 150]. Since discounted is returned and declared using let in the same scope, there are no scope issues. The loop logic iterates through the prices, then multiplies it by the discount factor (in this case 1 - 0.5 = 0.5), adding it to the new discounted list. Going from [100, 200, 300] returns [50, 100, 150].

9.  Similarly to question 5, line 11 throws a ReferenceError: i is not defined because i was declared using let inside the for loop, and this line attempts to access i outside the scope of the loop.

10. Line 12 prints 3 because length is declared as a const variable in the same scope as where it is printed, outside the for loop. Prices has 3 elements, so length is assigned prices.length = 3.

11. The function returns the list [50, 100, 150]. Since discounted is returned and declared using const in the same scope, there are no scope issues. The loop logic iterates through the prices, then multiplies it by the discount factor (in this case 1 - 0.5 = 0.5), adding it to the new discounted list. Going from [100, 200, 300] returns [50, 100, 150].

12. A. student.name
    B. student['Grad Year']
    C. student.greeting()
    D. student['Favorite Teacher'].name
    E. student.courseLoad[0]

13. A. The output is '32' because 2 is converted to '2' and concatenated with '3'.
    B. The output is 1 because '3' is casted to 3, then 2 is subtracted from it.
    C. The output is 3 because null is converted to 0 and subtracted from 3.
    D. The output is '3null' because null is converted to 'null' and concatenated with '3'.
    E. The output is 4 because true is converted to 1 and added with 3.
    F. The output is 0 because false and null are both converted to 0 and added with each other.
    G. The output is '3undefined' because undefined is converted to 'undefined' and concatenated with '3'.
    H. The output is NaN because '3' is converted to 3, while undefined is converted to NaN and subtracted from 3; any calculation involving NaN yields NaN.

14. A. The output is true because '2' is converted to 2, and 2 > 1 is true.
    B. The output is false because the first character '2' is lexicographically greater than '1'.
    C. The output is true because '2' is converted to 2, and 2 == 2 is true.
    D. The output is false because the comparison becomes between a number and a string when the strict equality operator (===) is used.
    E. The output is false because true is converted to 1, and 1 == 2 is false.
    F. The output is true because true is Boolean(2) is converted to true (since the argument is neither 0, -0, nor NaN), and true === true is true.

15. The equality operator (==) checks if two values are the same, and it allows for conversion. The strict equality operator (===) checks if two values are the same without conversion, meaning that it will always return false when comparing different types.

17. The function will return [2, 4, 6]. The function takes some array as input, iterates through each element, and applies the callback function to it before pushing it to an output array. In this case, the callback function passed in is doSomething, which returns double the input. For each element [1, 2, 3] of the input array, they are doubled and pushed to the newArr, which yields [2, 4, 6].

19. The code prints 1, followed by 4, followed by 3, then 2 (after a 1 second delay). 1 is printed, then 2 is placed on a queue to execute after 1 second, then 3 is placed on a queue to execute immediately after all the other normal instructions, then 4 is printed normally. 3 is then immediately printed, and 2 is printed after the 1 second delay.
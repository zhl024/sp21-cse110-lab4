 ## Part 1a
 1. values added: 20
 2. final result: 20
 3. values added: 20
 4. Returns an error. Since the variable result is declared by let, and thus it can only be accessed in the if block where it is defined in.
 5. Returns an error. Since the variable result is declared by const, and thus it cannot be reassigned. So the reassignment of it at line 9 causes an error.
 6. Returns an error. The program will not reach line 13 since it stops at line 9.

## Part 1b
1. print out 3 in the console, i is declared by var and therefore is available outside the for block. And function picks up a variable's latest change, which, in this case, is 3.
2. print out 150 in the console, discountedPrice is declared by var and therefore it is available outside the for block. Its latest change is 300*0.5=150.
3. print out 150 in the console, with similar reasoning, finalPrice is available, and its latest change is (150*100)/100=150.
4. The array discounted, which is [50, 100, 150]. The array discounted stores the discounted price. The variable discounted is declared by var and is an array. Then for first time in the for loop, 100*0.5=50 is pushed to discounted; second time 200*0.5=100; and third time 300*0.5=150.
5. It causes an error. Since the variable i is declared by let and inside the for block, i is not available outside the for block.
6. It causes an error. The variable discountedPrice is declared by let and inside the for block, thus discountedPrice is not available outside the for block.
7. print out 150 in the console, since finalPrice is declared outside the for  block. Thus, even if it is decalred by let, it is still available in line 14. And its latest change is 300*0.5=150.
8. The array discounted, which is [50, 100, 150]. Since the array discounted is declared outside the for block, even if it is declared by let, it is still available when returning it. Since the input price is [100, 200, 300] and the discount is 0.5. The resulting array storing discounted prices is [50, 100, 150].
9. It causes an error. Since the variable i is declared by let and inside the for block, i is not available outside the for block.
10. print out 3 in the console, length = the length of input array prices, which contains 3 elements. So length = 3. 
11. The array discounted, which is [50, 100, 150]. The variable discounted is declared by const. When we push values into discounted, we are not reassigning the constant. It is still the same reference, we are just adding to the array discounted, the constant reference. Thus it does not cause an error.
12. 
    1. student.name
    2.  student['Grad Year']
    3. student.greeting()
    4. student['Favorite Teacher'].name
    5. student.courseLoad[0]
13. 
    1. '32' since integers map to their exact string representation.
    2.  1 since strings are converted to numbers.
    3.  3 since null becomes 0 under the numeric conversion rules.
    4.  '3null' since null becomes 'null' under string conversion rules.
    5.  4 since true becomes 1 under numeric conversion rules.
    6.  0 since there is a mathematical operation: add between false and null. false becomes 0 and null also becomes 0 under numeric conversion rules.
    7.  '3undefined' since undefined becomes 'undefined' under string conversion rules.
    8.  NaN since undefined becomes NaN under numeric conversion rules.
14. 
    1. true since string '2' becomes a number 2.
    2. false. It is a comparison between strings, comparing the first character of both strings, '2' is greater than '1'. So '2' > '12'.
    3. true since string '2' becomes a number 2.
    4. false since === is strict equality and it checks equality without type conversion. 2 is an int and '2' is a string. They are of different types.
    5. true. Since all values other than 0 become true under boolean conversion rules.
    6. true. First, compare the type, true and Boolean(2) are both of boolean type. Then, Boolean(2) is true since 2 becomes true under boolean conversion rules. Thus the result is true.
15. == is a regular equality check, it checkes the equality with type conversion. Thus, == cannot differentiate 0 from false. === is a strict equality check, it checkes the equality without type conversion. Thus, it can tell the difference between 0 and false.
16. [answer](part1b-question16.js)
17. [2, 4, 6]. The first input parameter is [1, 2, 3], and the second parameter is the function doSomething. So step into the function modifyArray, initialize the constant array newArr, then get into the for loop. Inside the for loop, pushes the return value of doSomething() with input of i-th index of input array. The first index of array is 1, so times 1 by 2 and pushes to newArr. Repeat the process, we get [2, 4, 6].
18. [solution](part1b-question18.js)
19. 1 4 3 2. 
1. print `3`, because `i` is function scope and the loop condition is `i<3`, when loop ends `i=3`
2. print `150`, because `discountedPrice` is function scope, when loop ends `discountedPrice` = last calculated value = `prices[2] * (1 - discount)` = `150`
3. print `150`, similar reason to question 2. `finalPrice` = last calculated value = `Math.round(150 * 100) / 100` = `150`
4. `[50, 100, 150]`, before the loop `discounted` is a empty array, each execution in the loop will add a value to the array.
5. Error, because `i` is block scope(for block).
6. Error, bacause `discountedPrice` is block scope(for block).
7. print `150`, because line 14 and line 4 are in the same block, `finalPrice` = last calculated value = `150`.
8. `[50, 100, 150]`, before the loop `discounted` is a empty array, each execution in the loop will add a value to the array. There are no errors in the code, and no misuse of variables with the same name.
9. Error, bacause `i` is block scope(for block).
10. print `3`, bacause line 4 and line 12 are in the same block, `length` = `prices.length` = `3`.
11. `[50, 100, 150]`, no error because a variable with the const prevents it from being reassigned, but we can still manipulate it.
12. - A: `student.name`
    - B: `student['Grad Year']`
    - C: `student.greeting()`
    - D: `student['Favorite Teacher'].name`
    - E: `student.courseLoad[0]`
13. - A: `32`(string), in node `+` used for both arithmetic and string concatenation. `'3'` is a string and `2` is a number, so node converts `2` into `'2'` and concatenates them.
    - B: `1`(number), `-` used for arithmetic subtraction, so `'3'` is converted to `3`.
    - C: `3`(number), in this case `+` used for arithmetic addition, `null` is converted to `0`.
    - D: `3null`(string), in this case `+` used for string concatenation, `3` is converted to `'3'`
    - E: `4`(number), similar to question C, `true` maps to `1`.
    - F: `0`(number), when `+` used with booleans, boolean value converted to number, `false` maps to `0`, `null` converted to `0`.
    - G: `3undefined`(string), similar to question D, `3` is converted to `'3'`.
    - H: `NaN`, `-` used for arithmetic subtraction, but `undefined` is not a number, then the result is `NaN`.
14. - A: true, in this case `'2'` is converted to `2`.
    - B: false, `'2'` lexicographically greater than `'12'`.
    - C: true, node convert two operands to a common type, `2` converted to `'2'`.
    - D: false, two operands are different type, and node does not convert them.
    - E: false, `true` is converted to `1`, then the expression is equivalent to `1==2`.
    - F: true, `Boolean(2)` is true, node does not convert them, but `true===true`.
15. `==` convert two values to a common type then compares them. `===` compares them without type conversion.
16.
17. `[2, 4, 6]`, in function `modifyArray` the assignment is equivalent to `newArr.push(doSomething(array[i]))`, that is `newArr.push(array[i] * 2)`.
18.
19. `1 4 3 2`, first print `1` and `4`, then output `3` and `2` according to the order in the queue.
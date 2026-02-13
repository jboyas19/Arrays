# Arrays

## Instructions

1. Clone this repository down to your local machine. This will not be submitted.
2. Open the cloned folder with VS Code.
3. Live serve `index.html`.
4. Choose one person in the group to share their screen.
5. Everyone else should follow along and type the answers on their own computers.
6. As a team, read each question out loud and reach a consensus on the answer before moving to the next question.

## Access elements of an array

Much like strings, an **array** is a data type that can hold a _sequence_ of values.

```js
const numbers = [3, 2, 1, 1, 0];
```

| Index   | 0   | 1   | 2   | 3   | 4   |
| ------- | --- | --- | --- | --- | --- |
| Element | 3   | 2   | 1   | 1   | 0   |

1. What **element** is at index 1 of the array?
2. What element is at index 2 of the array (`numbers[2]`)?
3. What is the value of `numbers[4]`?
4. What index is the last element of an array with **length** 50?

```js
const heights = [76, 75, 79, 81, 77, 77, 75];
const words = ["A", "sentence", "contains", "words"];
```

5. Evaluate the following expressions:
   1. `heights[0]`
   2. `(heights[0] + heights[1]) / 2`
   3. `heights[0] + heights[1] <= heights[5] + heights[6]`
   4. `words[0] + heights[0]`
   5. `words[2][2]`
6. Why might a developer want to use an array instead of multiple variables?

## Iterate through an array

```js
const numbers = [0, 1, 1, 2, 3];
let i = 0;
while (i < numbers.length) {
  console.log("i:", i);
  i += 1;
}
```

7. What does `numbers.length` evaluate to?
8. What will the loop above print?
9. Modify the code to print the elements of the array.

We can also use a loop to populate an array, as follows:

```js
const badgers = [];
for (let i = 0; i < 10; i++) {
  badgers[i] = "badger";
}
```

10. What will the array `badgers` contain after the loop runs?
11. What is the final length of `badgers`?
12. Modify the code so that `badgers` will contain 2000 badgers after the code runs.
13. Why would a developer want to use a loop to initialize an array instead of **hard-coding** it?

## Mutate an array

```js
const fruits = [];
fruits.push("kiwi");
fruits.push("strawberry");
fruits.pop();
```

14. Run the lines of code above using the browser console to answer the following:
    1.  Does `push` add to the front or back of an array?
    2.  Does `pop` remove from the front or back of an array?
15. What is the syntax to call an **array method** (function)?
16. `shift` and `unshift` are very similar methods to `pop` and `push`.
    1.  Does `shift` remove from the front or back of an array?
    2.  Does `unshift` add to the front or back of an array?

## Use more array methods

```js
const words = ["A", "sentence", "contains", "words"];
const sentence = words.join(" ");
```

17. Run the lines of code above in the browser console to answer the following:
    1. What value is assigned to `sentence`?
    2. What is the type of `sentence`?
    3. Define what `join` does to an array. Be specific about input and output.
18. Search online and read documentation for the `slice` array method. With the same `words` array, write the line of code using `slice` that would return:
    1. `["contains", "words"]`
    2. `["A", "sentence"]`
    3. `["sentence", "contains", "words"]`

> [!IMPORTANT]
>
> There are _many_ more array methods! It would be unreasonable to memorize all of them. Instead, it is more important to learn how to find and read documentation about unfamiliar array methods.

## Practice writing code with arrays

19. At the top of `index.js`, create an array named `myInstruments` that contains the following instruments as strings: flute, clarinet, saxophone, trumpet, and trombone.
20. Use array methods to transform it into `["saxophone", "flute", "clarinet", "trumpet", "trombone", "tuba", "bassoon"]`.

> [!TIP]
>
> `splice` is an array method that allows you to remove elements from the middle of an array!

21. Complete the functions in `index.js` according to the provided JSDoc.

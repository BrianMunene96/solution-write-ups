# [Add Up Numbers](link-to-challenge)

Given a positive integer we can write a function that adds all numbers up to and
including that number

## Syntax

> addNumbers(`number`) -> `number`

### Parameters

**number**: `number`

- A number between 1 and infinity

### Return Value: `number`

- The sum of all numbers less than and equal to the given number added up

## Test Cases

```js
describe('Add numbers up to', () => {
  it('Should return 10 when 4 is passed', () => {
    expect(addUp(4)).toEqual(10);
  });
  it('should return 15 when 5 is passed', () => {
    expect(addUp(5)).toEqual(15);
  })
})
``` 

## Use Cases

- We can easily use this function to add all numbers up
to a certain point;

## Strategy

- Start by decl and init  a variable `sum` to store the sum
- Then use a `for loop` to iterate over a series of numbers equal and less to
  the given number. For each iteration add the number in the series to the `sum`
  and finally return the `sum`.

## Solution

```js
function addUp(num) {
  let sum = 0;
  for (let i = 1; i <= num; i++) {
    sum += i;
  }
  return sum;
}
```

## Retrospective

- There are very many different ways to arrive to the solution of a certain
problem. Some are short while some are long. The method used in my solution
takes a few more lines of codes while some of the solution I have seen are much
shorter.
- Ideally, the goal is to understand how a certain method works. This can then
can then allow you better understand other solutions which can be applied to
solve future problems

### Continue Doing

- Include two to three test for each function which can be nested within the
primary `describe`
- Compare your solution to the solution of others and see what you can pick up
from them

### Start Doing

- Check more background reading to have a better understanding of unit texting
- PRACTICE!!, PRACTICE!!, PRACTICE!!

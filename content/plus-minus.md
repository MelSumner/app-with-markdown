---
title: Plus Minus
author: Melanie Sumner
tags: algorithm
---

# Plus Minus

## Task

Given an array of integers, calculate the fractions of its elements that are positive, negative, and are zeros. Print the decimal value of each fraction on a new line.

## Code

```js
function plusMinus(arr) {
	let positiveNumsCount = 0;
	let negativeNumsCount = 0;
	let zerosNumsCount = 0;

	let totalNumsCount = arr.length;

	for (let ii = 0; ii < totalNumsCount; ii++) {
		if (arr[ii] > 0) {
			positiveNumsCount++;
		} 
		else if (arr[ii] < 0) {
			negativeNumsCount++;
		}
		else {
			zerosNumsCount++;
		}
	}
	console.log(positiveNumsCount / totalNumsCount);
	console.log(negativeNumsCount / totalNumsCount);
	console.log(zerosNumsCount / totalNumsCount);

}
```

## Ok but why?!

This demonstrates the ability to bucket sort things in an array. 

## Practical use(s)

- calculating loss/wins/draws for a sports app
- really anything else that needs sorting like this (there are lots, this one feels like it has obvious practical applications). 

## Reference

Hacker Rank problem: https://www.hackerrank.com/challenges/plus-minus/problem

DESCRIBE:luhnAl();

TEST: It should remove every other number from input.
CODE:let i = reversedInput.length;
while (i--) (i + 1) % 2 === 1 && (reversedInput.splice(i, 1));
EXPECTED OUTPUT:
reversedInput;
(8) [2, 5, 4, 6, 0, 0, 0, 4]

TEST: It should reverse order of input.
CODE:
const inputArray = [4, 1, 0, 2, 0, 8, 0, 8, 6, 0,4, 3, 5, 6, 2, 0];
const reversedInput = inputArray.reverse();
EXPECTED OUTPUT: reversedInput;
(16) [0, 2, 6, 5, 3, 4, 0, 6, 8, 0, 8, 0, 2, 0, 1, 4]

TEST: It should multiply every other number by 2 from right to left.
CODE:
reversedInput.map(function(number) {
  return number * 2;
});

EXPECTED OUTPUT: [4, 10, 8, 12, 0, 0, 0, 8]

TEST: It should add double digit number digits together
CODE: 

EXPECTED OUTPUT: [4, 1, 8, 3, 0, 0, 0, 8]


const sum = [4, 10, 8, 12, 0, 0, 0, 8].reduce((partialSum, a) => partialSum + a, 0);
console.log(sum);

const reversedInputArray = [4, 10, 8, 12, 0, 0, 0, 8]

var digits = reversedInputArray.toString().split('');
var realDigits = digits.map(Number)
console.log(realDigits);
[4, NaN, 1, 0, NaN, 8, NaN, 1, 2, NaN, 0, NaN, 0, NaN, 0, NaN, 8]

const sum =[4, NaN, 1, 0, NaN, 8, NaN, 1, 2, NaN, 0, NaN, 0, NaN, 0, NaN, 8].reduce((partialSum, a) => partialSum + a, 0);
console.log(sum);
VM2428:2 NaN

[4, 1, 0, 8, 1, 2, 0, 0, 0, 8]const reversedInputArray = [4, 10, 8, 12, 0, 0, 0, 8]
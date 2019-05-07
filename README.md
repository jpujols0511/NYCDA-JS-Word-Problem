# NYCDA-JS-Word-Problem

# Problem #1 - Reverse string 

function backwardString(str) {

    let separString = str.split("");

    let backwArray = separString.reverse();

    let combArray = backwArray.join("");

    return combArray;
}

console.log(backwardString('IamTheBestpRogRamEr'))

# Problem #2 Fizzbuzz using for loop

function fizzBuzz() {

  for (let i = 1; i <= 100; i++) {
    if (i % 3 == 0 && i % 5 == 0) {
      console.log('FizzBuzz');
    } else if (i % 3 == 0) {
      console.log('Fizz');
    } else if (i % 5 == 0) {
      console.log('Buzz');
    } else {
      console.log(i);
    }
  }
}
fizzBuzz()

# Problem #2 Fizzbuzz using while loop

function fizzBuzz2(){

  let i = 0

  while (i < 100){
    i++
    if (i % 3 == 0 && i % 5 == 0){
      console.log('FizzBuzz')
    } else if (i % 3 === 0){
      console.log('Fizz')
    } else if (i % 5 == 0){
      console.log('Buzz')
    } else {
      console.log(i);
    }
  }
}
fizzBuzz2()

# Problem #3 PigLatin Attempt

function pigLatinConverter(stringLatin){

let stringWord = stringLatin.toLowerCase().split(' ');
let pigLatinString = [];

let i = 0
while(i < stringWord.length){
  letters = stringWord[i].split('');
  letters.push(letters.splice(0,1)+' ay');
  newWordLatin = letters.join('');

  if(i === 0){
      newWordLatin = newWordLatin.slice(0,1).toUpperCase() + newWordLatin.slice(1);
    }

  pigLatinString.push(newWordLatin);
  i++
}

  pigLatinString = pigLatinString.join(' ');
  return pigLatinString;


}

console.log(pigLatinConverter('IamtheKing'))


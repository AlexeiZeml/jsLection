1)
1 undefined
2 const obj = { 
  name: 'Object', 
  getName () { 
	console.log (this.name) ; 
  } 
}; 
obj.getName();
2 
function greet(name){ 
  console.log(`${name}, ${this.name}!`);
}
const person = { name: 'Alice' };
greet.call(person,"hi")  ;
greet.apply(person,["fff"]);
const boundGreet = greet.bind(person,"xxx");
boundGreet();
1
let sum = (a, b) => {  
  let result = a + b;
  return result; 
};
console.log(sum(33,66));
2
let sum = (array) => {  
  return array.map((number) => number * 2);
};const number=[1,2,3,2,1];
console.log(sum(number));
3
const getStringLengths = (arr) => arr.map(str => str.length);
const strings = ["apple", "banana", "cherry"];
const lengths = getStringLengths(strings);

console.log(lengths); 

# .forEach, .map, .filter, .reduce, .find

For the following lesson please review [For Loops](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/for)!

Why write for loops over and over? they involve way too much writing, they're prone to syntactical errors. 

In the words of Jon Zachary: 

Terser Syntax => less typos => happier developers => world peace

## [.forEach()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/forEach)

Call the forEach method on any array, pass it a callback function which invokes three agruments(*Optional*): 
* the element value
* the element index
* the array being traversed

```javascript

const arr = ['a', 'b', 'c', 'd', 'e']

arr.forEach(function(el){
    console.log(el)
})

//expected output
=> 'a'
=> 'b'
=> 'c'
=> 'd'
=> 'e'

arr.forEach((d, i, a) => {
    console.log(`this is ${d}, this is the index ${i}, this is the array being traversed: ${a}`)
})

//expected output
=> "this is a, this is the index 0, this is the array being traversed: a,b,c,d,e"
=> "this is b, this is the index 1, this is the array being traversed: a,b,c,d,e"
=> "this is c, this is the index 2, this is the array being traversed: a,b,c,d,e"
=> "this is d, this is the index 3, this is the array being traversed: a,b,c,d,e"
=> "this is e, this is the index 4, this is the array being traversed: a,b,c,d,e"

```
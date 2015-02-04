# Two - camelCase

Keeping in mind the two functions we used yesterday, write a function named "toUpperCase" which takes a string as a single argument (don't worry about validation) and returns that string with the first letter capital.

```
 toUpperCase("hello world, my name is bes."); //--> "Hello World, My Name Is Bes."
 
```
**Solution: **

Adam's:

```
var testString = 'hello world whats up';

function toUpperCase(str) {
    var sentence = str.split(' '),
        word;
    for (var i=0; i<sentence.length; i++) {
        word = sentence[i].split('');
        word[0] = word[0].toUpperCase();
        sentence[i] = word.join('');
    }
    return sentence.join(' ');
}

console.log(toUpperCase(testString));

?:
```
```
function toUpperCase(sentence) {
    var wordsUpper = sentence.split(' ').map(function(word){
        var firstLetter = word.charAt(0).toUpperCase();
        var rest = word.slice(1);
        var complete = firstLetter + rest;
        return complete;
    });
    return wordsUpper.join(' ');
}

```


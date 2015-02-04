# Day 3

## Class Solution

```javascript
function toUpperCase(sentence) {
    var wordsUpper = sentence.split(' ').map(function(word){
        var firstLetterUpper = word.charAt(0).toUpperCase();
        var rest = word.slice(1);
        var complete = firstLetterUpper + rest;
        return complete;
    });
    return wordsUpper.join(' ');    
}

```

## Other Solutions

```javascript
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

```





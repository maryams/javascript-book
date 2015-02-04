# Day 7
## Recursive reverse string

```javascript
var test1 = "12345";
var test2 = "Hello World";

// Remove comments in function to see it in action
function reverseStr(str, ind) {
	ind = ind || 0;
	if (ind > str.length/2) {
		return str;
	}
	else {
		var letters = str.split('');
		var newLetters = [];
		for (var i=0; i<letters.length; i++) {
			newLetters.push(letters[i]);
		}
		// console.log('Before:');
		// console.log(letters);
		// console.log(newLetters);
		newLetters[ind] = letters[letters.length-(ind+1)];
		newLetters[letters.length-(ind+1)] = letters[ind];
		// console.log('After:');
		// console.log(letters);
		// console.log(newLetters);
		str = newLetters.join('');
		return reverseStr(str, ind+1);
	}
}

console.log(reverseStr(test1));
console.log(reverseStr(test2));
```

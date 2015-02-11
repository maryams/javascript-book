# Day 3

```
function once(func) {
var executed = false;
return function() {
if (!executed) {
executed = true;
return func();
}
}
}

var tryit = once(function(){console.log("executed");});

tryit();
tryit();

//Example
function asim(){
function will(){
return 7;
}
return will(); //this will return the execution of the function
return will; //this will return the function itself
}
var x = asim();
```
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
//this will return the execution of the function
return will(); 
//this will return the function itself
return will; 
}
var x = asim();
```

- functions are returnable values? 
- not all languages can return functions
- all functions return something, if you don't specify what, you return undefined
- **there is one return value per function scope**
- pass values from a sub scope to the scope above, you use a return
- `(!executed)` *read* false as true`
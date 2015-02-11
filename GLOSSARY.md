## Callback

A function that calls another function once the first function has completed.

A continuation function: You pass in the function that you want to continue after that operation is done. 

Imagine you're making a cup of tea. The asynchronous function that will take the longest time here is boiling the water. Once the water is boiled, you need to pour it. In this case, the callback is pouring the water.

TLDR, "Once something has happened, come back here and do this!"

function that calls a function, and allows you to define functionality of later on. not saying what it has to do. "i don't want to tell you how to use these properties, but I'm telling you that you should use them".

Javascript doesn't know anything is a function when an object is created? it's mapping out what to do in the future, not saying what to do right now. 


```
var http = {
    request: 10,
    response: 20,
    createServer: function(a, b, fn) {
        var x = a + b + prop;
        var y = a * b + prop2;
        return fn(y, x)
    }
}
```

##Call back hell/boomerang function

The end function is dirnking the cup of tea, but you may have many other functions e.g. putting the teabag in a cup, getting out the box of tea. You may have to sit down and write out stuff first. Don't use unnamed function callbacks. 

##.map()
test

##.filter()
test

## .split()
test

##.slice()
test

##.join()
test

##.charAt()

test
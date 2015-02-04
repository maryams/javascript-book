# Day 5
```javascript
/** 
 *    Create an object "bes", which has two methods. One method is named "sum" the other "sayHiTo".
 *    - method "sum" takes two arguments and returns a string with the sum (see example)
 *    - mehtod "sayHiTo" takes one argument and returns a string (see example)
**/

var bes = {
    sum : function(a,b) {
                        var result = a + b;
                        return "Result: " + result;
                        },
    sayHiTo : function(str) {return "Hi "+ str +"!"}
};

console.log(bes.sum(2,3)); // -> "Result: 5";
console.log(bes.sayHiTo("Dan")); // -> "Hi Dan!";

```

# Day 4 - chaining methods

- cleaner, quicker way to write things. smoother! no semi colons!

# Prototypes

# Objects

# Scope

## Private and Public Variables

- `new` keyword
- `this` keyword
- Global object
- pseudoclassical ??
- falsey && truthy
- that is a convention?
- constructors with the new and/or this keyword are harmful
- doing it explicitly is... not harmful?
- global vars are insecure
- this points to a global variable, can accidentally edit it!
- does everything inherit x? if you do it insecurely
- everyone working on the project can access the variables/methods/objects you were using = not secure
- **script injection**

```
function start ( startval ){
that = {}
that.value = startval || 0;

that.add = function() {
    that.value++;
    return that;
}

that.end = function() {
    return that.value;
}
return that;
};

```

#Solution

```
var start = function( startval ){

this.value = ( typeof( startval ) === 'number' )? startval : 0;
return this;
};

/start.prototype.start = function( startval ) {
this.value = ( typeof( startval ) === 'number' )? startval : 0;
return this;
}; /
start.prototype.add = function() {
this.value++;
console.log( 'add log: ' +this.value );
return this;
};

start.prototype.end = function() {
console.log( 'end log: ' +this.value );
return this.value;
};

//obj = new start();
var result = new start().add().end(); // will return 1
var result2 = new start().add().add().add().end(); // will return 3
```
Two:
```
var count = 0;

var start = function(num){
if (isNaN(num)==false){
count = num;
}
return obj2;
};

var obj2 = {
end:function(){
return count;
},
add:function(){
count += 1;
return obj2;
}
};
```

var result3 = new start(5).add().add().end(); // returns```
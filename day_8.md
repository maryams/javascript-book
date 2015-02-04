# Day 8

```var names =["bes", "izaak", "Dan", "nelson", "Ben", "natalia", "Beechware", "adam", "benjamin", "William", "ines"]; ```

```
if (!String.prototype.includes) {
String.prototype.includes = function() {'use strict';
return String.prototype.indexOf.apply(this, arguments) !== -1;
};
}

//console.log( names );
function typehead( searchString, searchArray ){
var search= searchString.toLowerCase();
return searchArray.filter( function( value, idx ){
console.log( value.toLowerCase() );
var lower = value.toLowerCase();
console.log( typeof( lower ));
return lower.includes( 'ben' );;
});
}

function typehead2( searchString, searchArray ){
var search= searchString.toLowerCase();
var lowerArray = searchArray.map( function( val, idx ){
return val.toLowerCase();
});
console.log( lowerArray );

return lowerArray.filter( function( value, idx ){
    console.log( value );

    return value.indexOf( search ) !== -1;
});
}

function typehead3( searchString, searchArray) {
lc = function( str ){
return str.toLowerCase();
};
return searchArray.filter( function(elm){
return lc(elm.slice( 0, searchString.length)) === lc(searchString);
})
}

console.log( typehead3('Ben', names) );```
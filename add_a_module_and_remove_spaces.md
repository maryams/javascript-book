# Add a module and remove spaces
```
// Challenge: please write a function that removes all spaces from
//the string passed to it. Please check that it is a string and not
//a different data type, ensure you use strict mode, and I would
//like you to save it as a module that you import and use in
//another file. (You will have to do this on your own environments,
//not on repl).

//the module itself 

module.exports = function spaceVoider() {
    "use strict";
    if (typeof myString === 'string') {
        return myString.replace(/\s/g, ' ');
    }
};

//the export line

var spaceVoider = require('./SpaceVoider');
```
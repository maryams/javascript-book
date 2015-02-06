```
// I have an app that lets me time how long I have been working for. 
// This is one of my time records: 

var t0 = {
    name: "Bes",
    createdTime: new Date("11 February 2012 15:30"),
    endTime: "NOW"
};

// I've just realised I started working 2 hours before I pressed start! 

var t1 = t0;

t1.createdTime = new Date("11 February 2012 13:30");

// If I check t0.createdTime here, it has also changed.

console.log(t0.createdTime); // --> 11 February 2012 13:30

// Uh oh, I just wanted to create a new version of the time, I didnt want to alter the old one!

// How would I created a new record of the time without deleting the old one? 
// (Because my employer will want to see where I have manually amended time records.)
// I would like a function that takes a time record object (in our case, t0) and returns a 
// cloned version that I will be able to modify without affecting t0 itself.
// REMEMBER: GOOGLE KNOWS MORE THAN ANYONE UPSTAIRS!
```
- for (var prop in obj) for in loop

#Prototypes
- inheritance
#Clones
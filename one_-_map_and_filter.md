# One - .map() and .filter()

---


Given a specific object which contains an array (look at list):

```
var data = {
    basket: "1",
    id: 1,
    list: [{
        id: 54,
        taste: "a"
    }, {
        id: 22,
        taste: "b"
    }, {
        id: 43,
        taste: "b"
    }, {
        id: 64,
        taste: "a"
    }, {
        id: 13,
        taste: "c"
    }, {
        id: 16,
        taste: "a"
    }, {
        id: 17,
        taste: "a"
    }]
};
```

**1. 
Return another array in which each element contains the id and index of each element in the list array.**

The result should look like this:

```
var a = [{
    indexPosition: 0,
    id: 54
}, {
    indexPosition: 1,
    id: 22
}, {
    indexPosition: 2,
    id: 43
}, {
    indexPosition: 3,
    id: 64
}, {
    indexPosition: 4,
    id: 13
}, {
    indexPosition: 5,
    id: 16
}, {
    indexPosition: 6,
    id: 17
}];
```

**2. 
From here create another array which will contains only the elements with id > 30.**

**Solutions**

**1:**

var a = data.list.map(function(element, index, list){
   return {"id": element.id, "index": index};
});

**2:**

var b = a.filter(function(e){
    return e.id >=30;```

});
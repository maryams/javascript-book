# Day 2

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

function list(obj) {
    myArr  = obj.list;
    result  = [];
    for (var i=0; i<myArr.length; i++) {
        result.push({});
        result[i].indexPosition = i;
        result[i].id = myArr[i].id;
    }
    return result;
}

function over30(arr){
    result = [];
    for (var i=0; i<myArr.length; i++) {
        if (arr[i].id > 30) {
            result.push(arr[i]);
        }
    }
    return result;
}

var a = list(data);
console.log(a);
var b = over30(a);
console.log(b);
```

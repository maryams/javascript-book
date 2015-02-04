# Morning Coding Problems

Hi everyone, I thought it would be good to compile the morning problems into a gitbook for future reference. 

Please add alternative solutions, and request notes if wanted.

------

challenge 5

not recursive:

```
function reverse(myString) {
    return myString.split('').reverse().join('');
    }
reverse("hello people");

```
# .reverse()

# .join()

# .splice()

arrays only

# .slice() 

**what's a recursive fuction?**
- always need an if function that will return false eventually
- always think of how you will exit it
- 

chicken and egg function?

**recursive function:**

function reverse(myString) {
    return reverse(myString);
    }
    
# Maximum call stack exceeded
 - memory of browser is full
 - infinite function
 - until the function is finished, it will not stop adding to the stack





# NectarScript Definition (NS)

## NS-v0.1

### Types

* Undefined
```javascript
var undef;
```
* Null
```javascript
var _null = null;
```
* Boolean
```javascript
var bool = false;
```
* String
```javascript
var string = "a string";
```
* Number (int)
```javascript
var number = 3;
```
* Array
```javascript
var arr = [0, "abc", [1,2,3]];
var aString = arr[1];
```
* Object
```javascript
var obj = {"key": "value", 0:1 };
var aString = obj.key;
```

### Semantics

* for
```javascript
for(var i = 0; i < 3; i++)
{
  console.log(i);
}
```
* while
```javascript
var i = 3;
while(i > 0)
{
  console.log(i);
  i--;
}
```
* do while
```javascript
var i = 3;
do
{
  console.log(i);
  i--;
}while(i > 0)
```

### Conditions

* if
```javascript
var i = 0;
if(i < 1)
{
  // code block here
}
```
* if / else
```javascript
var i = 0;
if(i < 1)
{
 // code block here
}
else 
{
 // code block here
}
```
* if / else if / else
```javascript
var i = 0;
if(i < 1)
{
 // code block here
}
else if(i == 2)
{
  // code block here
}
else 
{
 // code block here
}
```

### Operators

* \+
```javascript
var a = "string" + "string"; // "stringstring"
var b = "string" + 1; // "string1"
var c = 1 + 1; // 2
var d = 1 + "string"; // 0
var e = 1 + "string" + 2; // 2
```
* \-
```javascript
var a = 1-1; // 0
```
* /
```javascript
var a = 4/2; // 2
```
* \*
```javascript
var a = 2*2; // 4
```
* \%
```javascript
var a = 10%3; // 1
```
* \>
```javascript
var a = 1 > 0; // true
```
* <
```javascript
var a = 1 < 2; // true
```
* \>=
```javascript
var a = 1 >= 1; // true
```
* <=
```javascript
var a = 1 <= 1; // true
```
* \=
```javascript
var a = 1; // 1
```
* ==
```javascript
var a = 1 == 1; // true
```

### Functions

* Normal function
```javascript
function myFunc(x,y,z)
{
  console.log(x+1);
}
```
* Nested function
```javascript
function myFunc(x,y,z)
{
  function nestedFunction()
  {
    console.log(z); // same block
  }
  nestedFunction();
}
```


### Exceptions

* try/catch block

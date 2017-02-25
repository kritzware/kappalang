# kappalang

## Examples

### Variables/Assignment
```javascript
let x = 2;
let hello = "world";
let result = 10 * (20 / 2);

let array = [1, 2, 3, 4, 5];
let hashmap = {"status": 200, "error": false, "data": "xD"};

```

### Functions
```javascript
let multiply = fn(x, y) {
  return x * y;
}

let multiplyTwo = fn(x, y) { x * y };

multiply(5, 5); // => 25
multiplyTwo(5, 5); // => 25

let useless = fn(x) {
  if(x == 0) { 0 }
  else {
    useless(x - 1)
  }
}

useless(4) // => 0
```

### Higher Order Functions
```javascript
let first = fn(func, x) {
  return func(x);
}

let second = fn(x) { return x * 2 };

first(second, 2); // => 4
```

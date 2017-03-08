API:

### `array` Array.prototype.column (`index`)
Return the values from a single column

```javascript
[
    [1,2,3,4,5],
    [6,7,8,9,0],
    [1,3,4,6,9]
].column(0) // returns [1,6,1]
```
### `boolean` Array.prototype.empty ()
Truncate Array

```javascript
var a = [1,2,3,4,5,6,7,8,9,0];
a.empty();
console.log(a); // returns []
```

### `*` Array.prototype.end ()
> **IMPORTANT:** Alias of [last](#last)

Get the last item

```javascript
[1,2,3,4,5,6,7,8,9,0].end() // returns 0
```

### `boolean` Array.prototype.exists (`index`)
Check if item exists by index

```javascript
[1,2,3,4,5,6,7,8,9,0].exists(0)  // returns true
[1,2,3,4,5,6,7,8,9,0].exists(-1) // returns false
[1,2,3,4,5,6,7,8,9,0].exists(10) // returns false
[1,2,3,4,5,6,7,8,9,0].exists(9)  // returns true
```
### `*` Array.prototype.get(`index`, `_default`)
Get a item by index. If it not exists, return you own default value

```javascript
[1,2,3,4,5,6,7,8,9,0].get(0) // returns 1
[1,2,3,4,5,6,7,8,9,0].get(-1, false) // returns false
[1,2,3,4,5,6,7,8,9,0].get(-1) // returns undefined
```

### `boolean` Array.prototype.isEmpty ()
Check if a empty Array

```javascript
var a = [];
var b = [1,2,3,4,5,6,7,8,9,0];
a.isEmpty() // returns true
b.isEmpty() // returns false
```

### `boolean` Array.prototype.left (`index`)
Move item to left position by index

```javascript
[1,2,3,4,5,6,7,8,9,0].left(0); // returns [1,2,3,4,5,6,7,8,9,0]
[1,2,3,4,5,6,7,8,9,0].left(9); // returns [1,2,3,4,5,6,7,9,8,0]
```

### `boolean` Array.prototype.move (`from`, `to`)
Move a item by index position to a new index position

```javascript
[0,1,2,3,4,5,6,7,8,9].move(0, 9); // returns [1,2,3,4,5,6,7,8,9,0]
```
### `boolean` Array.prototype.remove (`index`)
Remove a item by index

```javascript
[1,2,3,4,5,6,7,8,9,0].remove(0); // returns true
// produces
// [2,3,4,5,6,7,8,9,0]
```

### `boolean` Array.prototype.right (`index`)
Move item to right position by index

```javascript
[1,2,3,4,5,6,7,8,9,0].right(0); // returns [1,2,3,4,5,6,7,8,9,0]
[1,2,3,4,5,6,7,8,9,0].right(9); // returns [1,2,3,4,5,6,7,9,8,0]
```

### `array` Array.prototype.shuffle ()
Shuffle array

```javascript
[1,2,3,4,5,6,7,8,9,0].shuffle();
```

### `*` Array.prototype.start ()
> **IMPORTANT:** Alias of [first](#first)

Get the first item

```javascript
[1,2,3,4,5].start() // returns 1
```

### `number` Array.prototype.sum ()
Calculate the sum of values

```javascript
[1,2,3,4].sum() // returns 10
```

### `boolean` Array.prototype.down (`index`)
> **IMPORTANT:** Alias of [right](#right)

Move item to right position by index

```javascript
[1,2,3,4,5,6,7,8,9,0].down(0); // returns [1,2,3,4,5,6,7,8,9,0]
[1,2,3,4,5,6,7,8,9,0].down(9); // returns [1,2,3,4,5,6,7,9,8,0]
```

### `*` Array.prototype.first ()
Get the first item

```javascript
[1,2,3,4,5,6,7,8,9,0].first() // returns 1
```

### `*` Array.prototype.last ()
Get the last item

```javascript
[1,2,3,4,5,6,7,8,9,0].last() // returns 0
```

### `boolean` Array.prototype.up (`index`)
> **IMPORTANT:** Alias of [left](#left)

Move item to up position by index

```javascript
[1,2,3,4,5,6,7,8,9,0].up(0); // returns [1,2,3,4,5,6,7,8,9,0]
[1,2,3,4,5,6,7,8,9,0].up(9); // returns [1,2,3,4,5,6,7,9,8,0]
```
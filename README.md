API:

### column
```javascript
[
    [1,2,3,4,5],
    [6,7,8,9,0],
    [1,3,4,6,9]
].column(0) // returns [1,6,1]
```
### empty
```javascript
[1,2,3,4,5,6,7,8,9,0].empty() // returns []
```
### end
```javascript
[1,2,3,4,5,6,7,8,9, 0].end() // returns 0
```
### exists
```javascript
[1,2,3,4,5,6,7,8,9,0].exists(0)  // returns true
[1,2,3,4,5,6,7,8,9,0].exists(-1) // returns false
[1,2,3,4,5,6,7,8,9,0].exists(10) // returns false
[1,2,3,4,5,6,7,8,9,0].exists(9)  // returns true
```
### get
```javascript
[1,2,3,4,5,6,7,8,9,0].get(0) // returns 1
[1,2,3,4,5,6,7,8,9,0].get(-1, false) // returns false
[1,2,3,4,5,6,7,8,9,0].get(-1) // returns undefined
```
### isEmpty
```javascript
[1,2,3,4,5,6,7,8,9,0].isEmpty() // returns false
[].isEmpty() // returns true
```
### left
```javascript
Array.prototype.column()
[1,2,3,4,5,6,7,8,9,0].left(0); // returns [1,2,3,4,5,6,7,8,9,0]
[1,2,3,4,5,6,7,8,9,0].left(9); // returns [1,2,3,4,5,6,7,9,8,0]
```
### move
```javascript
[0,1,2,3,4,5,6,7,8,9].move(0, 9); // returns [1,2,3,4,5,6,7,8,9,0]
```
### remove
```javascript
[1,2,3,4,5,6,7,8,9,0],remove(0); // returns true
// produces
// [2,3,4,5,6,7,8,9,0]
```
### right
```javascript
[1,2,3,4,5,6,7,8,9,0].right(0); // returns [1,2,3,4,5,6,7,8,9,0]
[1,2,3,4,5,6,7,8,9,0].right(9); // returns [1,2,3,4,5,6,7,9,8,0]
```
### shuffle
```javascript
[1,2,3,4,5,6,7,8,9,0].shuffle();
```
### start
Alias of [first](#first)

### sum
```javascript
[1,2,3,4].sum() // returns 10
```
### down
Alias of [right](#right)

### first
```javascript
[1,2,3,4,5,6,7,8,9,0].first() // returns 1
```
### last
```javascript
[1,2,3,4,5,6,7,8,9,0].last() // returns 0
```
### up
```javascript
Alias of [left](#left)
```
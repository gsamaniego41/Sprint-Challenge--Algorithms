Add your answers to the Algorithms exercises here.

## Exercise I

a)

```
n
  1

Time complexity: O(n)
Number of loops depend on the size of n.
```

b)

```
n
  n
    n
      n
n * n * n * n
Time complexity: O(n^4)
4 nested loops.
```

c)

```
Time complexity: O(n)
Number of items in n determine number of recursive calls.
```

## Exercise II

Binary search O(log n)<br />
Floors are already sorted by default<br />
Divide the number of floors by 2 `bldgA` + `bldgB`. <br />
Start with the bottom half `bldgA` <br />
Throw an egg from `floor 1` until we reach the top of `bldgA` <br />
&nbsp;&nbsp;&nbsp;&nbsp;If egg breaks before reaching the top of `bldgA`, iteration stops.
&nbsp;&nbsp;&nbsp;&nbsp;Else, move on to `bldgB` and repeat the process by dividing `bldgB` in half.

n story building
f floors
plenty of eggs
throw egg
if f > 2:
break egg
else:
egg doesn't break

```
bldg = n
mid = bldg / 2
bldgA =  bldg[0:mid]
bldgB =  bldg[mid:len(bldg)-1]
```

# Array Manipulation
[The link for the practice question can be found here][1]

##




## Answer 
** copying answers dont net you any learning, go try it for yourself first!**
scroll down for the answer
.
.
.
.
.
.
.
.
.
.
.
.
.
.
.
.
.
.
.
.
.
``` python
def arrayManipulation(n, queries):
    diffArray = [0] * (n+1)
    
    for q in queries:
        start, end, value = q
        start -= 1

        diffArray[start] += value
        diffArray[end] -= value

    maxDiff = 0
    currDiff = 0
    for change in diffArray:
        currDiff += change
        maxDiff = currDiff if currDiff > maxDiff else maxDiff

    return maxDiff
```


[1]: https://www.hackerrank.com/challenges/crush/problem?h_l=interview&playlist_slugs%5B%5D=interview-preparation-kit&playlist_slugs%5B%5D=arrays

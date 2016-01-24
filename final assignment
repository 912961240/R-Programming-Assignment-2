## Put comments here that give an overall description of what your
## functions do

##  This function creates a special "matrix" object that can cache its inverse.
## Argument x must be a matrix
## $set - sets the matrix
## $get - gets the matrix
## $setInverse - sets the inverse of the matrix
## $getInverse - gets the inverse of the matrix

makeCacheMatrix <- function(x) {
+        X.Inverse <- NULL
 +       set <- function(y) {
 +            x <<- y
 +            X.inverse <<- NULL
 +       }
 +       get <- function() x
 +       setInverse <- function(inverse) X.Inverse <<- inverse
 +       getInverse <- function() X.Inverse
 +       list(set = set, get = get,
 +            setInverse = setInverse,
 +            getInverse = getInverse)
 }

## Write a short comment describing this function

cacheSolve <- function(x, ...) {
        ## Return a matrix that is the inverse of 'x'
 +        X.Inverse <- solve(x, ...)
 +        x$setInverse(X.Inverse)
 +        X.Inverse
}

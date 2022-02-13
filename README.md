makeCacheMatrix <- function(x = matrix()) { 
  i <- Null, set <- function(y) 
  {x <<- y, i <<- NULL} get <- function() x
  setinverse <- function(inverse) 
  i <<- inverse, getinverse <- function() 
  i, list(set = set, get = get, setinverse = setinverse, getinverse = getinverse)}

x <- matrix(c(1, 2, 3, 4), 2, 2)
x
x1 <- makeCacheMatrix(x)
x1

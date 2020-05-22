## Exercise 3.9:

Define a procedure, absvalue, that takes a number as input and produces the absolute value of that number as its output. For example, (ab- svalue 3) should evaluate to 3 and (absvalue −150) should evaluate to 150.

Using built in function:

`(define (absvalue x) (abs x))`

Using if-else procedures:

    (define (absvalue num)
        (if (< num 0)
        (- num)
        num
    ))

**Explanation**:

If incoming `num` is lesser than 0, as expressed `(if (< num 0)` then return `num`. Otherwise return the `num` made negative with `(- num)`
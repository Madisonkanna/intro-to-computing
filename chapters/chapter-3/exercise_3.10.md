## Exercise 3.10:

Define a procedure, bigger-magnitude, that takes two inputs, and outputs the value of the input with the greater magnitude (that is, absolute dis- tance from zero). For example, (bigger-magnitude 5 −7) should evaluate to −7, and (bigger-magnitude 9 −3) should evaluate to 9.

## Solution:

I just ended up using the function I wrote for absolute value as a helper function.

    (define (absvalue num)
    (if (< num 0)
    (- num)
    num
    ))

and put it all together here:

    (define (bigger-magnitude x y)
    (if
    (> (absvalue x) (absvalue y))
    x y)
    )
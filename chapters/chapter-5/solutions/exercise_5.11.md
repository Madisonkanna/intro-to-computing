# Exercise 5.11

## Define a procedure is-list? that takes one input and outputs true if the input is a List, and false otherwise.

    (define (is-list? p)
    (if (null? p)
        true
        (if (pair? p)
            (is-list? (cdr p))
                false))
    
    )

*Explanation*: 
- If null, return `true`. 
- If there is a pair, recursively call `cdr` on the list until it is null, inevitably becoming `true`. Basically, `[1 2 3 4]` becomes `[2 3 4]` and then `[3 4]`.
 
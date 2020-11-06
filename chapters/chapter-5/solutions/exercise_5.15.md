# Exercise 5.15

## Define a procedure list-last-element that takes as input a List and outputs the last element of the input List. If the input List is empty, list-last- element should produce an error.

    (define (lastGuy p)
    (if (null? p)
        (error "Index Out Of Range")
        (if (null? (cdr p))
            (car p)
            (lastGuy (cdr p))))
    )

    (lastGuy (list 4 2 0 69))
# Exercise 5.12

## Define a procedure list-max that takes a List of non-negative numbers as its input and produces as its result the value of the greatest element in the List

1) Brute force method:

    (define (list-max p)
    (if (null? p)
        0
        (if (> (list-max (cdr p)) (car p))
            (list-max (cdr p))
            (car p)
            )) 
    )

2) Using previously declared `bigger` method

    (define (bigger a b) (if (> a b) a b))

    (define (list-max2 p)
    (if (null? p)
        0
    (bigger (car p) (list-max2 (cdr p))))
    )
# Exercise 5.9

## Another way of thinking of a triple is as a Pair where the first cell is a Pair and the second cell is a scalar. Provide definitions of make-triple, triple- first, triple-second, and triple-third for this construct.

Triple Definition:

    (define (trip-scal a b c)
        (cons (cons a b) c)
    )

Lookup Functions:


    (define (triple-first t) (car (car t)))
    (define (triple-second t) (cdr (car t)))
    (define (triple-third t) (cdr t))

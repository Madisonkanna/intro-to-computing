# Exercise 5.8

## Define a procedure that constructs a quintuple and procedures for selecting the five elements of a quintuple.

Using the original built in procedures, I can use `cons`, `car`, and `cdr` to build this procedure.

    (define (make-quint a b c d e)
        (cons (cons a b)(cons (cons c d) e))
    )

*NOTE: For odd numbered collections, it is easier to make the first cell a pair using the cons procedure, while the second cell could be the scalar type*.

The individual lookups:

    (define (quint-uno t) (car (car t)))
    (define (quint-dos t) (cdr (car t)))
    (define (quint-tres t) (car (car (cdr t))))
    (define (quint-quatro t) (cdr (car (cdr t))))
    (define (quint-cinco t) (cdr (cdr t)))


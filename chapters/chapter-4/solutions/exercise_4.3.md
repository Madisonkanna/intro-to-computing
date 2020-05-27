# Exercise 4.3

## Define a procedure `fcompose3` that takes three procedures as inputs, and produces as output a procedure that is the composition of the three input procedures.

Given that the following have already been defined:

`(define (square x) (* x x))`

`(define (cube x) (* x x x))`

### A) once without using fcompose:

    (define ((threeFunctions func1 func2 func3) input)
        (func3 (func2 (func1 input)))
    )


### B) using fcompose:

    (define (fcompose3 func1 func2 func3)
        (lambda (input) (func3 (func2 (func1 input))))
    )

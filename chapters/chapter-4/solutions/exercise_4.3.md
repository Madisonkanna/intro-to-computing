# Exercise 4.3

## Defineaprocedurefcompose3thattakesthreeproceduresasin- put, and produces as output a procedure that is the composition of the three input procedures.

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

*NOTE: Obviously, there are a lot of ways to write these functions, whether using `lambda` or not, and using the naming conventions `xyz` as you see in the book. I chose this way because it is a lot clearer in my head when I use real words.
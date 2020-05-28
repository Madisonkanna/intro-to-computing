# Exercise 4.4

## Define a f2compose procedure that composes two procedures where the first procedure takes two inputs, and the second procedure takes one input. 

    (define (f2compose func1 func2)
        (lambda (x y) (func2 (func1 x y)))
    )
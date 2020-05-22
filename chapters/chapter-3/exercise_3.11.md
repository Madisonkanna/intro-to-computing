## Exercise 3.11:

Define a procedure, biggest , that takes three inputs, and produces as output the maximum value of the three inputs. For example, (biggest 5 7 3) should evaluate to 7. Find at least two different ways to define biggest , one using bigger, and one without using it.

## Solutions:

1) Using if else:

    (define (biggest a b c)
        (if (> a b)
            (if (> a c) a c)
            (if (> b c) b c)
        )
    )

2) Using bigger

- Helper function here:

`(define (bigger a b)(if (> a b) a b))`

    (define (biggest a b c)
        (bigger a (bigger b c))
    )
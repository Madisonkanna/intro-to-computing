# Exercise 4.6

## Define a recursive procedure,gauss-sum, that takes a number n as its input parameter, and evaluates to the sum of the integers from 1 to n as its output. For example, (gauss-sum 100) should evaluate to 5050.

    (define (gauss-sum n)
        (if (= n 1) 1
            (+ n (gauss-sum (- n 1))))
    )

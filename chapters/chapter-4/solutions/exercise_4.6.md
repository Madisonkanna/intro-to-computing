# Exercise 4.6

## Define a recursive procedure,gauss-sum, thattakes a numbernas its input parameter, and evaluates to the sum of the integers from 1 tonasits output. For example, (gauss-sum100) should evaluate to 5050.

    (define (gauss-sum n)
        (if (= n 1) 1
            (+ n (gauss-sum (- n 1))))
    )

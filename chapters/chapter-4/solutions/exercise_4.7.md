# Exercise 4.7

## Define a higher-order procedure, accumulate, that can be used to make both gauss-sum (from Exercise 4.6) and factorial. The accumulate procedure should take as  its  input  the  function  used  for  accumulation  (e.g., ∗ for factorial,+ for gauss-sum).  

    (define (accumulate f)
        (lambda (n)
            (if (= n 1) 1
                (f n ((accumulate f) (- n 1)))))
    )

# Exercise 4.7

## Define a higher-order procedure,accumulate, that can be used tomake bothgauss-sum(from Exercise 4.6) andfactorial. Theaccumulateprocedure should takeas  its  input  the  function  used  for  accumulation  (e.g.,∗forfactorial,+forgauss-sum).  

    (define (accumulate f)
        (lambda (n)
            (if (= n 1) 1
                (f n ((accumulate f) (- n 1)))))
    )

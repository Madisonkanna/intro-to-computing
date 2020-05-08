## Exercise 3.3
### Using DrRacket to evaluate Scheme expressions

#### A) Seconds in a year:

`(* 365 (* 24 (* 60 60)))`

#### B) Seconds I've been alive:

`(* 32 (* 365 (* 24 (* 60 60))))`

Or, using a definition:

`(define (secs-lifetime age) (* age (* 365 (* 24 (* 60 60)))))`

#### C) Fraction I've been in school:

Function definition:

`(define (frac-school age years) (/ years age))`

That returns a fraction. Using the following to give a decimal equivalent, I can see that I spent over half my life in school:

`(exact->inexact (frac-school 32 18))`
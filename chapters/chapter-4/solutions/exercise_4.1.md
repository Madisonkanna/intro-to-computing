# Exercise 4.1

## For each expression, give the value to which the expression evaluates.  Assume _fcompose_ and _inc_ are defined as above.

a. ((_fcompose square square_)3)

### Solution a

This application expression (_fcompose square square_) evaluates to a procedure that composes _square_ w/_square_ (multiplying the input by itself 4 times). Applying this procedure to **3** evaluates to **81**.

b. (_fcompose_(__lambda__(_x_) (_*x_ 2)) (__lambda__(_x_) (_/x_ 2) ))

### Solution b

This evaluates to an identity procedure for numerical inputs. This produces a procedure which accepts a number as its input, which in turn  applies a procedure that multiplies by **2** to the result of a procedure that divides the input number by **2**.

c. ((_fcompose_(__lambda__(_x_) (_∗x_ 2) ) (__lambda__(_x_) (_/x_ 2)) ) 1120)

### Solution c

This applies the identity procedure from the previous example to 1120, so the result is 1120.

d. ((_fcompose_(_fcompose inc inc_)_inc_)2)

### Solution d

The inner application expression, (_fcompose inc inc_), evaluates to a procedure that takes a numerical value as its input and outputs the result of incrementing it twice. The next expression, (_fcompose_(_fcompose inc inc_)_inc_), composes with another inc procedure, resulting in a procedure that adds **3** to its input. Applying this procedure to **2** results in the value of **5**.


## Exercise 3.2

**a)** `1120`

- I assumed this would simply return the value.
- In DrRacket:

![Exercise3.2a](/chapters/chapter-3/images/Ex3.2a.png)

**b)** `(+ 1120)`

- Without anything to add to that `+` primitive expression, I would get back the 1120.

![Exercise3.2b](/chapters/chapter-3/images/Ex3.2b.png)

**c)** `(+ (+ 10 20) (* 2 0))`

- For this one, I approached it following the orders of operations from grade school. The inner parenthesis would go first, with 10 being added to 20 to make 30. And 2 to be multipled by 0, to get zero. These values are then added according to outer level `+`, to get 30.

![Exercise3.2c](/chapters/chapter-3/images/Ex3.2c.png)

**d)** `(= (+ 10 20) (* 15 (+ 5 5)))`

- Now, taking a gander at prior notes within the textbook, I assumed that `=` sign asks whether the evaluated sums from inner parentheses are equal. `+ 5 51` is 10, which is multiplied by the `* 15` to get 150. And `(+ 10 20)` would just be 30. So, no. They are not equal.

DrRacket's answer (*drumroll...*):

![Exercise3.2d](/chapters/chapter-3/images/Ex3.2d.png)

*Note:* The interpreter spits out an anticlimactic `#f` which apparently means False. Some extra reading was found here: [CS#431: Scheme Basics](https://courses.cs.washington.edu/courses/cse341/02wi/scheme/basics.html).

**e)** `+`

- I honestly didn't expect anything to come out of this, maybe a keyword requiring me to peruse the Scheme Basics once more. I was wrong.

DrRacket's answer:

![Exercise3.2e](/chapters/chapter-3/images/Ex3.2e.png)

**f)** `(+ + <)`

- For this one, I tried to be intuitive about what the procedure was trying to evaluate. `+` and `+` together are not lesser than nothing. Maybe equal, but that would require me to deep dive into what equality actually means in Scheme.

DrRacket's answer:

![Exercise3.2f](/chapters/chapter-3/images/Ex3.2f.png)
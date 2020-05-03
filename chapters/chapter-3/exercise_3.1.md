## Exercise 3.1

*Note:* In the book, triangles are used instead of showing the complete parse tree for nested application expressions. I don't know how that works in markdown, so I use `<>`

                                            *Expression*
                                                  |
                                        *ApplicationExpression*
                                            |       |       |
    (   *Expression*                                      *MoreExpressions*                                                  )
             |                                                    |
    *PrimitiveExpression*                           *Expression*                        *MoreExpressions*
             |                                            |                                     |
           **+**                                *PrimitiveExpression*            *Expression*                  *Expression*            
                                                          |                            |                            |
                                                       **100**               *ApplicationExpression*            *ApplicationExpression*
                                                                                       <>                                <>
                                                                                    **(* 5)**                        **(+ 5 5)**

And in DrRacket:

    ![Exercise3.1](/images/Exercise3.1png)

**Note:** When evaluating the above with the DrRacket IDE, it's important to have `lang Scheme` stated at the top of the document. Otherwise, we run into the error:

                Module Language: only a module expression is allowed, either
                    #lang <language-name>


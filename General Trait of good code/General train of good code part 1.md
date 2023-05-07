# Desing by contract

## Pre conditions

These are the codition which are required the function before calling the function
Validation logic can be put in client side or server side(demanding approach) but it is safe to put the logic in demanding approach

## Post conditions

It guarantees that after processing the request certain properties are preserved in return data.

We can add control mechanism(ValueError,SyntaxError) to enforce the contract

### Note

If a single condition is unmet the program will raise error. This is more about making the code able to protect themselves against invalid inputs.

In next part we will study about the Defensive programming

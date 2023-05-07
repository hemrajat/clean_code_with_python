# Defensive Programming

Main idea here is how to handle the errors for scenarios that we might expect to occur, and how to deal with error that should never occur

## Approaches of handling errors

1. ### Value Substitution
   We replace the missing value with default value or safer value
   ```python
   import os
   host = os.getenv('host',3000) 
   # If host doesn't exist in environment variable the default value 3000 will be returned
   ```
2. ### Exception Handling
   Notifing the caller of the function that something is wrong and clearning stating what went wrong with proper logging
   #### Note
   a. exceptions should be used for—clearly announcing an exceptional situation, and not altering the flow of the program according to business logic
   b. Dot not disclouse traceback to end user since it show the function callback history this might lead to breach in intellectural property and security issue
# termMachine
## Initialization
raw text file

## Features
### Property
    * term: get the terms of each machine
    * tf_dict: get the tf of every word in the machine

### Function
    * save: save the result.
    ```
    @target: store the result to a file, whose name is defined in FileName
    ---
    @param fileName : the name of the file, in which you want to store the result in
    @param method   : the method that the result is store, there are two options, and the default is 'w'.
        > 'a': - Append - will create a file if the specified file does not exist
        > 'w': - Write - will create a file if the specified file does not exist
    @param sep      : the word that split the result, default is '\\n'
    ---
    @raise ValueError(method): thrown when the user input the invalid method symbol.
    ```

# Prospect
* use lambda expression in the termMachine.processing to allow user to customize their tokenize rule.

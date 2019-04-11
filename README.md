# NFA to DFA Converter

## Description

This program converts a given NFA with epsilon movements to an equivalent DFA.

## Usage

After downloading, run `make` in the downloaded directory.

![alt text](README_images/make.png)

After running it, you will find the executable 'automata_conversion.out'. To run it, execute the command `./automata_conversion.out`.

![alt text](README_images/run.png)

It will then ask you to input two strings:

1. The path of the input file. An example of a valid input is: `NFA_example.txt`.

![alt text](README_images/input_filepath.png)

2. The path of the output file. An example of a valid input is: `DFA_solution.txt`.

![alt text](README_images/output_filepath.png)

You will then see the message `Output written successfully!` if the execution was correct.

![alt text](README_images/result.png)

## Input file format

The input file should be as follows (each part should be written with a newline character):

1. __State amount__: The number of states the automata has. An example of a valid input is `10`. 
    * The actual states will be considered to start at 0.
    * If you have 10 states, then the states would range from 0 to 10.
    * The NFA initial state will always be considered to be 0.

2. __Alphabet size__: The size of the alphabet used in the automata. An example of a valid input is `3`. 
    * Should be an integer with a maximum value of 5. 
    * The alphabet will always be considered to start with the epsilon character.
    * The alphabet, if its size is greater than 2, would then be followed by the character 'a', 
    and subsequently end with the character 'd'.

3. __Final states amount__: The amount of final states the NFA has. For example: `1`.

4. __Final states__: The actual final states, listed one per line. For example `9`.

5. __Transition amount__: The amount of transitions that will be specified for the NFA, one per line. 
Each transition will be specified as follows (elements separated by spaces):
    1. Initial node
    2. Final node
    3. Symbol
    
    An epsilon movement should be specified with the character `f`.
    
    Examples of valid transitions are as follows:
    
   1. 0 1 f
   2. 0 3 f
   3. 1 2 a 


There is also an example of this file format in the `NFA_example.txt` file in the project directory.    

## Output

The output will be written in the specified path and will have the same format as the input file.

 ## Author
 
 Axel Zuchovicki - ITESM CSF

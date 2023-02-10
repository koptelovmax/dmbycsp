# Explanations for Data Mining by Constraint Programming
The code to support our IDA'23 paper "Explanations for Itemset Mining by Constraint Programming: A Case Study using ChEMBL data"

### Structure of the code:

- **ac3_backtrack_dm_emerging_closed.py** -- emerging closed itemset mining (chi-square)

- **ac3_backtrack_dm_emerging_closed_minfreq_maxtaille.py** -- emerging closed itemset mining (chi-square) with min frequency and max pattern size constraints

- **ac3_backtrack_dm_emerging_closed_minfreq_maxtaille_pure.py** -- emerging closed itemset mining (chi-square) with min frequency, max pattern size and pure solution constraints

- **ac3_backtrack_dm_emerging_closed_minfreq_maxtaille_pure_expl.py** -- explanations for emerging closed itemset mining with min frequency, max pattern size and pure solution constraints, verification of constant constraints

- **solution_check.py** -- basic statistics on solution (pattern size, coverage, frequency)

### How to run the code from the terminal:

Data mining by constraint programming:

*python3 'program_name' 'dataset_name' 'transactions' 'transaction_classes' 'parameters'* (see comments in each program for examples)

Basic statistics:

*python3 solution_check.py 'dataset_name' 'total_number_transactions'* (see comments for examples)

Environment requirements: Python 3.8.8, numpy, intertools

Data must be place into 'data' directory. Sets from [1] can be used for benchmarking (need to be open with *loadDBFromFile(file)* function).

------------------------------------------------------------
References:

[1] T. Guns, S. Nijssen, L. De Raedt. Itemset mining: A constraint programming perspective, Artificial Intelligence 175(12-13), 2011

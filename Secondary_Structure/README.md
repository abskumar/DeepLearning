# Protein Secondary Structure Prediction

### This is a simple attempt to predict secondary structure (helix/strand/coil) from the primary sequence of the protein.

### The data was obtained from PDB (https://www.rcsb.org/pages/download/http#ss) and processed as below:

- ***parse_ss.ipynb:*** read PDB data and make a csv file containing the sequence, secondary structure, length. The output is saved in ss_data.csv
- ***generate_ss_data.ipynb:*** Split ss_data.csv by length. Additionally, split longer sequences for any structure into smaller lengths (6,7,8,9,10)
- ***ss_predict.ipynb:*** uses ss_data_length_8.csv to predict the secondary dtructure from sequences of length 8

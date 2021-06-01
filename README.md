### MPCS-56420 Final Project

#### Edris Qarghah

#### 06/01/2021

##### How to Run

This project is an web visualization of the Needleman-Wunsch and Smith-Waterman sequence alignment algorithms. To run locally, first make sure you're in an environment running python3, then `pip install -r requirements.txt`. You can then simply run `main.py`.

You can also find the project online for the time being, hosted [here](https://seismic-hope-272623.uc.r.appspot.com).

##### Functionality

Input any two sequences of arbtrary length. Once submitted, an empty table will populate and you can specify the algorithm, scoring matrix and gap cost. After doing so, you can step through the process of filling in the table, either a cell or a row at a time. If you select to Fill the entire table, you can then begin tracing the highest scoring alignment.

For Needleman-Wunsch (global alignment), this will start in the bottom right corner in the table and will proceed to the top right (arrows are not displayed on the for the first row (all come from the value to their left) and first column (all come from the cell above them). For Smith-Waterman, it will start at the maximum value across the entire table and trace back until it hits a zero.

##### Known funkiness

I appear to unintentionally be saving some details between runs. This means that if you change the sequence alignment, for example, your trace-back arrow may be wrong for a single frame.
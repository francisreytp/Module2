# Challenge
Refactored Code for Stock Analysis

* In our original code we idendified the names of the stocks and used it as a filter for the 'for'(i) loops.
   * Underneath these loops we run another 'for'(j) loops that went from the beggining-row to the end-row of our data set.

* Our data set is comprised of 3012 rows. A lot of our secondary 'for'(j)loops are unnecessary because it does not carry the  
  value of that stock (on that particular 'for'(i) loop). 
   * Thousands of row are not included in every instance of the 'for'(i)loop, or for every stock. 
   * We have 12 stocks, so tens and of thousands of commands are not useful for the operation.
     
* On the refactored code, each row of data only ran on the new 'for'(j)loop once.
   * It identifies the initial occurence of a stock to the last to project the information that we asked for.
   * It then moves on to the following row to start calculating the next stock. None of the previous rows needs to run in the 
     loop agian. Then again it records the calculation on the last occurence of the stock on the data sheet.
   * Each of the 3012 row will only run once in the refactored loops saving the computer tens and thousands of procedure.

Download Link: https://assignmentchef.com/product/solved-col226-assignment-4-integrating-the-earlier-assignments-into-a-simple-spreadsheet
<br>
Assignment 4: Integrating the earlier assignments into a simple spreadsheet

In Assignment 4: you will implement the backend, type-check the operations, and integrate the entire work.

You will need to check that the operations on rows, columns and ranges (especially in type 2 operations) are of consistent dimensions (two ranges being added should be of the same size).

You need to write clear specifications of the OCaml functions which you implement, and document your code.

Backend

In order to evaluate the above functions, you might want to implement the following in OCaml:

<ul>

 <li>full count: sheet -&gt; range -&gt; index -&gt; sheet : Fills count of valid entries in the given range into the specified cell</li>

 <li>row count: sheet -&gt; range -&gt; index -&gt; sheet : Fills count of valid entries per row in the given range into the column starting from the specified cell col count: sheet -&gt; range -&gt; index -&gt; sheet : Fills count of valid entries per column in the given range into the row starting from the specified cell.</li>

 <li>full sum: sheet -&gt; range -&gt; index -&gt; sheet : Fills the sum of entries of cells in the given range into the specified cell</li>

 <li>row sum: sheet -&gt; range -&gt; index -&gt; sheet : Fills the sum of entries of cells per row in the given range into the column starting from the specified cell</li>

</ul>




<ul>

 <li>col sum: sheet range    index -&gt; sheet : Fills the sum of entries of cells per column in the given range into the row starting from the specified cell</li>

 <li>full avg: sheet range    index -&gt; sheet Fills the average of entries of cells in the given range into the specified cell</li>

 <li>row avg: sheet range    index -&gt; sheet : Fills the average of entries of cells per row in the given range into the column starting from the specified cell  col avg: sheet range    index -&gt; sheet Fills the sum of entries of cells per column in the given range into the row starting from the specified cell</li>

 <li>full min: sheet -&gt; range -&gt; index -&gt; sheet : Fills the min of entries of cells in the given range into the specified cell</li>

 <li>row min: sheet -&gt; range -&gt; index -&gt; sheet : Fills the min of entries of cells per row in the given range into the column starting from the specified cell col min: sheet -&gt; range -&gt; index -&gt; sheet : Fills the min of entries of cells per column in the given range into the row starting from the specified cell</li>

 <li>full max: sheet -&gt; range -&gt; index -&gt; sheet : Fills the max of entries of cells in the given range into the specified cell</li>

 <li>row max: sheet -&gt; range -&gt; index -&gt; sheet : Fills the max of entries of cells per row in the given range into the column starting from the specified cell col max: sheet -&gt; range -&gt; index -&gt; sheet : Fills the max of entries of cells per column in the given range into the row starting from the specified cell</li>

 <li>add const: sheet -&gt; range -&gt; float -&gt; index -&gt; sheet : adds a constant to the contents of each cell in the selected cell range</li>

 <li>subt const: sheet -&gt; range -&gt; float -&gt; index -&gt; sheet : subtracts a constant from the contents of each cell in the selected cell range mult const: sheet -&gt; range -&gt; float -&gt; index -&gt; sheet : multiplies the contents of each cell in the selected cell range by a constant.</li>

 <li>div const: sheet -&gt; range -&gt; float -&gt; index -&gt; sheet : divides the contents of each cell in the selected cell range by a constant.</li>

 <li>add range: sheet -&gt; range -&gt; range -&gt; index -&gt; sheet : adds the cell contents for each corresponding pair of cells in two selected cell ranges</li>

 <li>subt range: sheet -&gt; range -&gt; range -&gt; index -&gt; sheet : performs a subtraction on the cell contents for each corresponding pair if cells in two selected cell ranges mult range: sheet -&gt; range -&gt; range -&gt; index -&gt; sheet : multiplies the cell contents for each corresponding pair of cells in two selected cell ranges</li>

 <li>div range: sheet -&gt; range -&gt; range -&gt; index -&gt; sheet : performs a division on the cell contents for each corresponding pair of cells in two selected cell ranges</li>

</ul>
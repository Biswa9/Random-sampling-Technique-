
1. *Worksheet and Columns*:
   - The code assumes that the Claim ID is in Column A. Adjust claimCol, randomCol, rankCol, and sampleCol to match your actual columns.
   - randomCol stores random numbers generated by the RAND() function.
   - rankCol stores the rank of these random numbers.
   - sampleCol is where the script marks rows selected for audit.

2. *Random Numbers*:
   - The code generates a random number for each row in the dataset, except the header.

3. *Ranking*:
   - The RANK formula is used to rank these random numbers from highest to lowest.

4. *Selecting Top 10%*:
   - The top 10% of the ranked rows are marked with "Audit" in the sampleCol column.

### How to Use:
1. Open Excel.
2. Press Alt + F11 to open the VBA editor.
3. Insert a new module (Insert > Module).
4. Copy and paste the code into the module.
5. Close the VBA editor.
6. Run the macro (Alt + F8) and select RandomAuditByClaimID.

The macro will select 10% of the rows randomly based on the Claim ID and mark them as "Audit" in the designated column. 
This approach uses both Excel functions and VBA to automate the process.

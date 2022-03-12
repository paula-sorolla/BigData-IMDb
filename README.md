# BigData-IMDb


## ACTIONS

### Years

Make Years into integers (int16) before/when storing them in the DB 
When reading them for our model they should be transformed into strings since they are a categorical feature

### Label

Make Label in a 0 - 1 format to further reduce strain on the db and processing(Maybe smth better)

### Votes

Make Label in a int32 when storing


### Titles

Varchar will be used in the DB no options here

### Ttconst

Keep only the digits that are useful and use these instead of the useless information of characters

### General

1.The manipulations should be done in the least amount of passes possible

2.Every /N should be turned to null, since /N is a character and that occupies uneeded space and also makes our in memory usage bigger for no reason

3.Drops should be done with bigger priority in order to reduce further memory strain


**Attention**

***If the above can NOT be accomplished in a small amount of passes then the whole procedure is useless since we add overhead instead of making the process faster, caution needed.***



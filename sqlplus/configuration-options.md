There some useful preferences that you can set in your `login.sql` or `glogin.sql` that will help you use sqlplus inside your shell scripts.

`set linesize 30000` : This is used to set the width of each page in your sql results
`set pagesize 30000` : This is used to set how many line will be printed by page in your sql results
`set pagesize 0`: This set the pagesize to infinite
`set wrap off` : Truncates the line if its is longer then LINESIZE. This should not happen if linesize is large enough.
`set trimspool on` : Set it otherwise every line in the spoolfile is filled up with blanks until the linesize is reached.
`set trimout on` :  Set it otherwise every line in the output is filled up with blanks until the linesize is reached.
`set feedback off` : To remove the "x lines were updated" at the end of sql results.

All commands can be used in any sql file and in the interactive sqlplus prompt as well. But it if you always will use this configuration it is better to put in `login.sql`
or even `glogin.sql`

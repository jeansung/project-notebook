### Final week ending December 12th

### Worklog
|Day | Time | What I did|
|:---|:-----|:---------|
| 12/8/14| 30 minutes | Set up github pages website rearranged info from readme |
| 12/9/14 | 1 hour | Alejandro final write up critique | 
| 12/9/14 | 1 hour 30 minutes | Critique reflection, figured out what I need to do this week. Cleaned up out of date files. Cleaned up code with comments. Created bash script to activate the virtual environment and run the program. Allowed white space in table file.  |

<!--
Tonight:
error handling
Test the bash file 
test the bash file on another mac
update instructions to include the bash file  
revise instructions / remove duplicates 
 -->
 
<!--
 Instructions:
 - bash script is what will run your thing! 
-allowed white space in table creation
-if you are getting an error on the  word, look for the comma 
- if the shell scripts are not running then use chmod +x scriptName to add execute, may need to execute as sudo 
-->

### Critique reflection
Alejandro tested my program this week and gave me advice on how to wrap up my final deliverable even better. He also gave helpful feedback in what is not currently well implemented, the error messages. I agree that the problem is better solved by good error messages rather than combining the table and rule file, because the anticipated use case is that people will write multiple set of rules per table). I will be sure to focus on adding error messages this week in addition to work relating to wrapping the project up. 


### Week work plan

| Task | Detail |
|:-----|:-------|
| Beef up error handling| Add error handling and helpful feedback for the common mistakes (e.g. when people write rules that reference types that don't exist or missing last comma). |
| Allow tables to have extra white space | Add in a rstrip to post facto remove the white space | 
| Revise instructions | Add in new shell file to activate the virtual environment and call `run.py` for the user. Clarify that the table and the rule files must be made before hand. | 
| Dream version | Figure out what the dream version of the project looks like (i.e. web interface) and compare what you have created this semester | 
| Clean up repository | Remove duplication of instructions and `README.md` files caused by having a README document and a `gh-pages` branch | 
| Clean up documents folder | Include final version of grammar, remove out of date files | 
| Clean up code | Add comments where necessary | 
| Final write up of the project | As specified by online requirements| 
| Test the code on another mac that is NOT mine | To make sure that all the dependencies work | 

### Future work / not going to support
- having a current/target progress bar for the values in the Excel sandbox (because I am not entirely sure what this would look like for the type based rules)
- validation checker (checking for contradiction of rules) 
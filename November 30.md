# Design notebook for week ending November 30, 2014

## Description

**TODO:** Fill in this part with information about your work this week:
important design decisions, changes to previous decisions, open questions,
exciting milestones, preliminary results, etc. Feel free to include images
(e.g., a sketch of the design or a screenshot of a running program), links to
code, and any other resources that you think will help clearly convey your
design process.

This week, I finished connecting the parsed rules to actionable Excel formulas. I am still working on actually writing the rules to the Excel worksheet and making instructions, but the parts are all there. I also finished the evaluation.md file. 

To see a sample of what I am talking about, you can download this repo as a zip file and navigate into the `program files` directory. From there, you can run:

```
python generateSandbox.py newtable.txt SAMPLE12
python generateConstraints.py test_rules.txt SAMPLE12SUPPORT.txt
```
Running the first command should give you an excel file that you can play around in. The `test_rules.txt` file in the second command is where you can write rules. Make sure not to reference any type that is now given in the `newtable.txt` file. Running the second command gives you the rules in the terminal. They work if you copy them to the original Excel sheet and put double quotes around okay, bad. Then put an equal sign in front of the `IF`. 

## Questions

**What is the most pressing issue for your project? What design decision do
you need to make, what implementation issue are you trying to solve, or how
are you evaluating your design and implementation?**

Linear programming is the most pressing issue. I would like to get the contradiction checking for my rules to work and this is what is holding it up. 


**What questions do you have for your critique partners? How can they best help
you?**

Do you know anything about linear programming in Python? Python support for it?

**How much time did you spend on the project this week? If you're working in a
team, how did you share the labor?**

|Day | Time | What I did|
|:---|:-----|:---------|
| 11/25/14| 1 hour 30 minutes | Critique for Alejandro project, including downloading/installing and testing some of the components |
| 11/26/14 | 45 minutes | Logo brainstorm and creation, integrate it with the project |
| 11/26/14 | 45 minutes | Meeting with Prof Ben to discuss how to implement the contradiction checking |
| 11/26/14| 30 minutes | Revision of the grammar and parser as per Alejandro's suggestion |
| 11/26/14| 1 hour 15 minutes | Revised test cases for new parser and split along more files | 
| 11/29/14| 3 hours | Connecting parser with creating rules for excel |
| 11/30/14| 4 hours | Reorganizing the code/ refactoring, adding in Excel support for type rules, more user testing, initial thoughts for the evaluation.md file |
| 11/30/14| 2 hours 15 minutes | Finished excel support for value rules, project notebook, evaluation.md file | 
| Total | 14 hours | 


## Post-critique summary

Alejandro's critique was very enlightening this week because he showed me how I could better structure my parser such that the parsed rules actually had useful components that I could use to create the Excel formulas. He also suggested a better way for me to structure and create test cases, which is helpful and will save me some time. 

## Post-critique reflection

I already mentioned the ways that Alejandro helped me this week. I also talked to Prof Ben about the idea for consistency checking for my rules (i.e. that there are no contradictions) and linear programming seems to be the answer. MatLab's `linprog` and `intlinprog` seem to be the functions that I am looking for and I know that NumPy has something similar but this requires more research. 

**Planned work**  
* research linear programming methods in Python
* revise the grammar and parser
* reorganize the code and move utility 
* connect rules to excel file 
* `evaluation.md` file 

**Actual work**  
I did everything I planned. Well, I still need to write the Excel formulas to the excel worksheet. Right now, you can only see them in terminal. But they do work!  I could have done more for the research on linear programming. I also didn't have time to clean up the front end of what I did, i.e. writing instructions, so I will be sure to do that soon.  


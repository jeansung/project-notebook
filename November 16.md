# Design notebook for week ending November 16, 2014

## Description

**TODO:** Fill in this part with information about your work this week:
important design decisions, changes to previous decisions, open questions,
exciting milestones, preliminary results, etc. Feel free to include images
(e.g., a sketch of the design or a screenshot of a running program), links to
code, and any other resources that you think will help clearly convey your
design process.


The major things I did this week was to create a grammar for the rule creation. I also flushed out what the system architecture is. I also designed a prototype that interfaces python with Excel to show that what I need to be done, can be done. Finally, I created a rough screen recording of the pre prototype product just to give a run through of how my thing works right now.

[Grammar](https://github.com/jeansung/project/blob/master/work%20products/prelim_grammar.md)  
[System architecture](https://github.com/jeansung/project/blob/master/work%20products/system_architecture_picture.jpg)   
[Link to current code](https://github.com/jeansung/project/blob/master/Excel%20prototypes/createTable.py)   
[Pre prototype](https://drive.google.com/drive/#folders/0B9z84Or5GzOnQnNKdm1pY01GMUU)     



## Questions

**What is the most pressing issue for your project? What design decision do
you need to make, what implementation issue are you trying to solve, or how
are you evaluating your design and implementation?**

The most pressing issue for my project this week is getting feedback on the grammar I created for my rules. A big deal for my prototype is to show that the grammar is viable to parse rules from that I can enforce in the python code. 

**What questions do you have for your critique partners? How can they best help
you?**

Questions I have for my critique partner- is the grammar okay? I am trying to make it wide enough to cover the cases that are explained in the `constraints.txt` document but small enough to manageable. I am also not really sure how the parsed form of the rule looks like ... 

**How much time did you spend on the project this week? If you're working in a
team, how did you share the labor?**

|Day | Time | What I did  |
|:---|:-----|:---------|
| 11/11/14 | 1 hour | Went to Prof Ben's office to get a better idea of what my project looks like language wise and how to move forward. |
| 11/11/14 | 1 hour | Critique for Alejandro project |
|11/13/14 | 1.5 hour | Post critique, reflection, plan for the week, started the design and implementation document | 
| 11/13/14 | 2.5 hours | Design & implementation document, proof of concept in Excel |
|11/13/14| 0.5 hours  | working on Excel prototype, error strapping | 
|11/15/14 | 1 hour 15 minutes | Excel prototype, creating intermediate types | 
| 11/15/14| 2 hours | Finished excel prototype with simple rules | 
|11/15/14| 3.5 hours | Developed grammar for rule generation, design architecture, finished design and implementation document, update README, took screen recording for the pre prototype, finished project notebook entry for this week |
| Total time | 13.25 hours | 

## Post-critique summary

At the time of writing this, Alejandro hasn't done an official critique in my critiques folder, but I got really helpful feedback from him in class during our critique group session. I presented my dilemma of having a way to 
* statically define the table
* statically define the rules 
* bring everything together to let the user in a sandbox experiment to see what works and what doesn't given a set of defined constraints

People in my group helped me see that I should funnel the rules and the table through Python to output an Excel document. This would let the user play in the Excel (which would live update).   

## Post-critique reflection

I went to Prof Ben's office hours to help get a resolve for the structure of my language. This diagram shows how a statically defined table, and a set of statically defined rules (which takes a valid table, and does a set of error checking), and feeds this into Python for the intermediate representation of (Table, List[Rule]). This gets compiled to an Excel file, which the user can do things from.

![](https://github.com/jeansung/project/raw/master/work%20products/language_things.jpg)

From this diagram, the hard part of the process seems to be
* grammar of the rules 
* method creating the rules (i.e. the interface)
* parsing the rules and tables to create an IR
* outputting the IR to excel 

On this project, I want to focus on 
* grammar of the rules
* parsing the rules and tables to create an IR

If I have time, my stretch goals can be creating a nice interface for the user to input the rules, but after I create a grammar for this, I anticipate that being more side work, as opposed to part of the fundamental structure of the language. 

**Planned work**
This week, the language and implementation design document is due.  I am working on
* creating a grammar for the rules (I have started this process somewhat last week by listing out what are the types of constraints I plan to support)
* creating a proof of concept of taking things from Python to Excel
	* this means that my deliverables this week will have code!
	* I will definitely get the table from text to Python to Excel
	* A stretch goal is to translate rules (parsed into the grammar) to Excel (I know that Excel supports formulas )
* finishing the implementation and design document 

Looking a bit ahead, the prototype is due next week. I have a fully functioning output in Excel, and I plan to do a very simple use case (probably with hard coded rules) that goes from text to python to Excel. 

**Actual work**

This week, I have finished everything I have planned to do, including:
* created a grammar for the rules (in `preliminary_grammar.md`)
* created a proof of concept in Excel
	* reads in types, values to generate initial tables
	* generates intermediate tables
	* enforces a total sum of values rules
	* does all this from text/python to Excel sandbox
* finished implementation design and implementation document, i.e. the `design_and_implementation.md` document
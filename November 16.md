# Design notebook for week ending November 16, 2014

## Description

**TODO:** Fill in this part with information about your work this week:
important design decisions, changes to previous decisions, open questions,
exciting milestones, preliminary results, etc. Feel free to include images
(e.g., a sketch of the design or a screenshot of a running program), links to
code, and any other resources that you think will help clearly convey your
design process.

## Questions

**What is the most pressing issue for your project? What design decision do
you need to make, what implementation issue are you trying to solve, or how
are you evaluating your design and implementation?**

**What questions do you have for your critique partners? How can they best help
you?**

**How much time did you spend on the project this week? If you're working in a
team, how did you share the labor?**

|Day | Time | What I did  |
|:---|:-----|:---------|
| 11/11/14 | 1 hour | Went to Prof Ben's office to get a better idea of what my project looks like language wise and how to move forward. |
| 11/11/14 | 1 hour | Critique for Alejandro project |

|11/13/14 | 1 hour | Post Critique Summary, reflection, plan for the week | 

## Post-critique summary

At the time of writing this, Alejandro hasn't done an official critique in my critiques folder, but I got really helpful feedback from him in class during our critique group session. I presented my dilemma of having a way to 
* statically define the table
* staticially define the rules 
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
	* I wil definitely get the table from text to Python to Excel
	* A stretch goal is to translate rules (parsed into the grammar) to Excel (I know that Excel supports formulas )
* finishing the implementation and design document 

Looking a bit ahead, the prototype is due next week. I have a fully functioning output in Excel, and I plan to do a very simple use case (probably with hard coded rules) that goes from text to python to Excel. 

**Actual work**
# Design notebook for week ending November 23, 2014

## Description

**TODO:** Fill in this part with information about your work this week:
important design decisions, changes to previous decisions, open questions,
exciting milestones, preliminary results, etc. Feel free to include images
(e.g., a sketch of the design or a screenshot of a running program), links to
code, and any other resources that you think will help clearly convey your
design process.

The biggest thing I accomplished this week was starting the parser for my language. I revised the EBNF grammar from last week with some suggestions, and researched which parser I would want to use. I decided on using PyPEG parser and started work on creating the parser and some of the test cases that come along with the parser.  These files can be found in the `program files/parsing` folder in my main directory and the thoughts can be found in the `work products/thoughts` folder. 

Here is a [link](https://drive.google.com/a/g.hmc.edu/file/d/0B9z84Or5GzOnaXhDMXFVLUpaOUk/view?usp=sharing) to the video that does a mini walkthrough of the prototype. 

The document that contains the prototype write up can be found in the `work products` directory. 


## Questions

**What is the most pressing issue for your project? What design decision do
you need to make, what implementation issue are you trying to solve, or how
are you evaluating your design and implementation?**

The most pressing issue for my project this week is the parser. I need to make sure that it is functional and fully featured before I focus on tying the functionality to the parser in the next couple of weeks. 

**What questions do you have for your critique partners? How can they best help
you?**

My main questions this week surround the parser - how does it look? The suggestion for which parser to use was helpful from last week, but now I would like help seeing if things inside the `program files/parsing` folder make sense. Am I missing something?

**How much time did you spend on the project this week? If you're working in a
team, how did you share the labor?**


|Day | Time | What I did|
|:---|:-----|:---------|
| 11/17/14| 1 hour 15 minutes | Critique for Alejandro project |
| 11/20/14 | 30 minutes | Talked with Prof Ben about rule grammar, got feedback for grammar and suggestion for implementation |
| 11/21/14 | 3 hours | Made improvements to grammar based on Alejandro's suggestions <br> Post critique summary and reflection <br> Spent time researching both parser choices, picked pyPEG and started to attempt to read up on how to use it |
| 11/23/14 | 30 minutes | More research on PyPEG and what I am trying to accomplish with the grammar |
| 11/23/14 | 2 hours 15 minutes | Parser research and development |
| 11/13/14 | 2 hours | Created deliverables for prototype  <br> Test cases for parser <br> Folder cleanup / update README <br> Project Notebook |
| Total time | 9.5 hours ||  


## Post-critique summary

Alejandro gave me a really good critique this week, the feedback was especially helpful because the grammar is a big part of the language part of this project. 

I changed the grammar a bit based on the feedback - especially adding support for decimal numbers, which I think was an important distinction I did not initially include. The wording suggestion also made sense so I changed it, but I am not worried about it really because the wording should be grammar independent and those words not in parenthesis will probably be hard coded into the interface that is presented to the user. 

Also, based on the feedback, I changed the program to have only 2 input files, one for the table (types that are comma separated on 1 line, values that are common separated on the next) and one for the rules. I think comma separated is a more natural way of specifying types and values, so that works out. I don't think one file is enough because I want to allow users to have different sets of rules per table. I agree to clean up the code because this would be good for the upcoming prototype / code review. 


## Post-critique reflection

This week the prototype for the language is due. Also, implicitly due is some decent code because we are doing code review in class on Monday /Wednesday. 

**Planned work**

* improved the grammar from the feedback
* research python parsers (Prof Ben suggested [this](https://pypi.python.org/pypi/grako/3.4.2) and Alejandro suggested [this](http://fdik.org/pyPEG/)
* code hygiene (move code to utility files) 
* create something for the prototype - I have code that I could show but it would be cool to have something parser related 
* Bonus: start the parser

**Actual work** 

I did everything I planned to do this week except for the code hygiene in terms of moving the utility functions of the `generateSandbox.py` file into a separate file. Since the main focus of my work this week was the parsing, I spent time polishing those files with test cases instead. The `generateSandbox.py` does have comments and well labeled functions, even if it is a bit long. I will try and get to the code cleanup over Thanksgiving Break. 


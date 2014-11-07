# Design notebook for week ending November 9, 2014

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

|Day | Time | Work log |
|:---|:-----|:---------|
| 11/3/14 | 1 hour | Critique (reading github repo contents and answering questions) for Alejandro |

1 hour Friday morning
2 hours Friday night 

## Post-critique summary
*For the critique from November 4th*  
Alejandro pointed out that the main engineering work can be done by Excel (the idea of weighted sum and doing logical IFs for constraints). The challenge will be to create a good, useable interface for entering inputs of the constraints for my target audience, non programmers. This means making good error messages syntax and logical, possibly including a constraint checker that checks for contradictory rules and reports which one is contradictory. 


## Post-critique reflection

Alejandro helped me a lot this week, especially showing me the capabilities of Excel. This is very helpful for my project because this means that all of the functionalities can be fully done in Excel, and now my job will be focused on language design, making sure that the user interface is friendly and that error messages are user friendly and actually helpful. 

Projected work:  
The deliverable for the end of this week is finding a host language and proper implementation tools. I know that Excel will at least be a large part of my toolkit but I will take some time to explore better and more non programmer friendly ways to generate and input constraints. Projected tasks include
* flush out all the (the small set of) use cases for my language that I want to support (i.e. the set of all types of constraints I want to start with)
* implement a proof of concept mock up in Excel
* think about user end design and brainstorm better/more intuitive ways to input the/ generate the constraints 
* explore options for the host language, focusing on making sure that inputting/presenting the interface is easy
	* possibly web related
	* possibly Java Applet (I have familiarity with Java Swing/ Fx) 
	* 

Looking ahead to next week, the deliverable is language design and implementation overview. I have some answers for the language design part, and I will make sure to use this document as a guide when I do this week's work. I am less clear about how what I am doing counts a language, in terms of the traditional syntax - IR - semantics model and I am going to meet with Prof Ben to clear that up soon so that when it comes time to implement the semantics / parser, I have a clear idea of what I hold to accomplish. 


Actual work:


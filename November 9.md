# Design notebook for week ending November 9, 2014

## Description

**TODO:** Fill in this part with information about your work this week:
important design decisions, changes to previous decisions, open questions,
exciting milestones, preliminary results, etc. Feel free to include images
(e.g., a sketch of the design or a screenshot of a running program), links to
code, and any other resources that you think will help clearly convey your
design process.


I did a lot of research this week on language designs /UI design and the result of those research can be found in `ui_design.md` in the `work products` folder.

This week, I created a preliminary prototype that can be found in [this](http://www.amazon.com/gp/product/B00MVDPLDK/ref=ox_sc_act_title_2?ie=UTF8&psc=1&smid=A11MLNV5RSJZCI) Excel file. 


My open question this week is how I am going to resolve the putting together the pieces question, more details of which can be found in `to_resolve.md` in the `work products` folder.


## Questions

**What is the most pressing issue for your project? What design decision do
you need to make, what implementation issue are you trying to solve, or how
are you evaluating your design and implementation?**

The most pressing issue I am trying to fix is that I need to figure out is how to put the pieces together.  I think I have an idea of what I want to accomplish in terms of the program flow of the language as elaborated upon in the works product folder. 


**What questions do you have for your critique partners? How can they best help
you?**

I don't really have any specific questions for my critique partners this week. They can best help me by looking at the proposed program flow/ use case in Part 1 of `to_resolve.md` in the `work products` folder and giving feedback on whether it makes sense for a typical user or not. 

**How much time did you spend on the project this week? If you're working in a
team, how did you share the labor?**

|Day | Time | What I did  |
|:---|:-----|:---------|
| 11/3/14 | 1.5 hours | Critique (reading github repo contents and answering questions) for Alejandro |
|11/7/14| 1 hour | Spent time writing the post critique summary and planning |
|11/9/14| 2 hours | Flushed out the small use cases for the language, i.e. what constraints I was going to support, started mockup in Excel | 
|11/9/14| 2 hours | Finished mockup in Excel and did research on what UI Design, language considerations / what I am stuck on (to formalize getting help on Tuesday for Prof Ben) | 
|11/9/14| 2 hours | Finished notebook reflection entry, updated project README, started considering the answers for the questions next week| 
|Total  | 8 hours | | 

<!--I know this is not the required 9 hours per week. I was swamped with interviews (3) and an midterm, which made it hard to progress before the weekend. Next week, I will hopefully have more time earlier in the week. -->


## Post-critique summary
*For the critique from November 4th*  
Alejandro pointed out that the main engineering work can be done by Excel (the idea of weighted sum and doing logical IFs for constraints). The challenge will be to create a good, useable interface for entering inputs of the constraints for my target audience, non programmers. This means making good error messages syntax and logical, possibly including a constraint checker that checks for contradictory rules and reports which one is contradictory. 


## Post-critique reflection

Alejandro helped me a lot this week, especially showing me the capabilities of Excel. This is very helpful for my project because this means that all of the functionalities can be fully done in Excel, and now my job will be focused on language design, making sure that the user interface is friendly and that error messages are user friendly and actually helpful. 

**Projected work:**  
The deliverable for the end of this week is finding a host language and proper implementation tools. I know that Excel will at least be a large part of my toolkit but I will take some time to explore better and more non programmer friendly ways to generate and input constraints. Projected tasks include
* flush out all the (the small set of) use cases for my language that I want to support (i.e. the set of all types of constraints I want to start with)
* implement a proof of concept mock up in Excel
* think about user end design and brainstorm better/more intuitive ways to input the/ generate the constraints 
* explore options for the host language, focusing on making sure that inputting/presenting the interface is easy
	* possibly web related
	* possibly Java Applet (I have familiarity with Java Swing/ Fx)  

Looking ahead to next week, the deliverable is language design and implementation overview. I have some answers for the language design part, and I will make sure to use this document as a guide when I do this week's work. I am less clear about how what I am doing counts a language, in terms of the traditional syntax - IR - semantics model and I am going to meet with Prof Ben to clear that up soon so that when it comes time to implement the semantics / parser, I have a clear idea of what I hold to accomplish. 


**Actual work:**

This week I finished all of the projected work that I planned to do in the projected work section. I didn't make it to any decisions, but I did work out what sort of questions I need to ask my critique partner/ my professor to narrow down my options. 

 
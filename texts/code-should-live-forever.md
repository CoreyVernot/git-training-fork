**What does it mean for code to "stay alive"? It means that *any other researcher* can run it *without errors* and obtain *consistent results***. To achieve this, code should be written to endure: plan your analytic workflow having in mind that it may be used again and again. It may seem otherwise, but implementing good practices as soon as you start writing code will save you time. It will also make coding more pleasant!

**A common practice that prevents code from staying alive is requiring a series of manual steps to run the code or re-create outputs**. For example, projects where one needs to open and run different pieces of code in a particular order, where code is typed directly into a software’s console, or where users need to copy-paste inputs from one software to another – copy-pasting from statistical software to word documents being the most common offense. To avoid this issue, follow the [guidelines on automation discussed below](https://devinnovationlab.github.io/guides/principles/coding.html#automate-your-workflow-from-the-start){:target="_blank"}.

**Another common practice that hinders endurance is neglecting transferability and creating code that only runs in one computer**. For example, by hard coding file paths or using libraries that are not installed on other machines. Strategies that can help prevent this include:

- *Sharing all the necessary operating system configurations alongside the code through containers*. This is the safest way to guarantee a smooth transfer between computers, but it can also be costly to set up and requires specific software for code to be reused. 
- *Making it easy to adjust file paths*.
- *Setting up a system to manage packages and user-written commands*, including the specific versions used. This can be done in Python using virtual environments, in R with the `renv` package, and in Stata by sharing the code for the command versions used. 
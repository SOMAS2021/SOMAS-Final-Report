# SOMAS Final Report

## Structure

This repository includes the following elements:
- A main file containing the used packages, the layout and the main document  itself, where every chapter is included using the command `\input{folder_name/name_of_chapter}`
- A folder for every chapter. The name of every folder begins with the chapter number. Inside every folder, a TeX file and another folder named "images"
- The file "latex_guidelines.md", which contains additional guidelines regarding the use of LaTeX (figures, notations, ...)
    - >TODO: Create latex_guidelines.md (see [Issue #7](https://github.com/SOMAS2021/SOMAS-Final-Report/issues/7))

## GitHub Guidelines

The following guidelines apply to this GitHub repository:

- Commits should be made to a separate branch and merged to main via a PR.
- PRs must be reviewed by someone in the editor team.
  - >TODO: Define who will be in the editor team.
- Do not approve your own pull requests.
- Pull requests have a pipeline which compiles the PDF. You can see the compiled document in the PR by going to `Checks` and then `Artifacts`

## Writing Guidelines

The separate file "latex_guidelines.md" gives you important guidelines and reminders on how to use LaTeX, so that we can achieve consistency and correctness in the final report.

It is important that your writing is correct and consistent.

You should review your writing for correct spelling, grammar, and punctuation.

## Figures, Tables and Equations

Figures should add to the text. Redundant figures should be removed since they can confuse the reader and distract them from the important points in the text.

Figures, tables and similar objects should always be talked about in the text. They also need to be refered to by figure number and not position.
e.g. 
- Good - "as you can see in Figure 6"
- Bad  - "as you can see in the figure below"

Equations should be refered to using their equation number with parenthesis around the equation number.
e.g. 
- Good - "as shown in (6)"
- Bad  - "as shown in Equation 6"
- Bad  - "as shown in the equation below"
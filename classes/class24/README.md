# 431 Class 24: 2020-11-19

[Main Website](https://thomaselove.github.io/431/) | [Course Calendar](https://thomaselove.github.io/431/calendar.html) | [Syllabus](https://thomaselove.github.io/431-2020-syllabus/) | [Course Notes](https://thomaselove.github.io/431-notes/) | [Piazza & TA Office Hours](https://thomaselove.github.io/431/contact.html) | [Canvas](https://canvas.case.edu) | [Data and Code](https://thomaselove.github.io/431/data_index.html)
:-----------: | :--------------: | :----------: | :---------: | :-------------: | :-----------: | :------------:
for everything | for deadlines | expectations | from Dr. Love | ways to get help | zoom information | for downloads

## XKCD on [Prediction](https://xkcd.com/2370/)

![](https://imgs.xkcd.com/comics/prediction.png)

## Today's Slides

- Class 24 slides are available in [PDF format](https://github.com/THOMASELOVE/431-2020/blob/master/classes/class24/431_class-24-slides_2020.pdf), as well as in [R Markdown](https://github.com/THOMASELOVE/431-2020/blob/master/classes/class24/431_class-24-slides_2020.Rmd).

## Announcements

1. Results of Minute Paper after Class 23 **to come**.
2. Status report on Project B Study 2 Data Plans (due today at noon) [can be found here](https://github.com/THOMASELOVE/431-2020/blob/master/projects/projectB/study2-dataplan-status.md).
3. I've updated [the R Packages list](https://thomaselove.github.io/431/r_packages.html) to include `equatiomatic`. If you include `equatiomatic` in your loaded packages, it will generate a warning if you haven't upgraded to R version 4.0.3. Feel free to use `warning = FALSE` to suppress that warning if you're still using R 4.0.2. (Yes, this means you can use `warning = FALSE` to fix this in loading packages for your Project B.)
4. Regarding NHANES for Study 2 in Project B, I made a [short video](https://github.com/THOMASELOVE/431-2020/blob/master/projects/projectB/README.md#video-to-help-you-deal-with-some-common-nhanes-issues) where I pulled some data from NHANES 2017-18, merged it, and then changed  values like "Refused" or "Don't Know" in a variable to missing values. The video is now linked in [the Project B instructions](https://thomaselove.github.io/431-2020-projectB/your7.html), too. A few other comments based on the study 2 data plans:
    - Some binary variables are coded 1 and 2. Fix that in your work, ideally by using the real names and treating the variable as a factor, or by converting the 1-2 to a proper 1-0 indicator variable.
        - Use the formula **NEWVAR = 2 - OLDVAR** to turn OLDVAR: 1 = Yes, 2 = No into NEWVAR: 1 = Yes, 0 = No.
        - If you have OLDVAR: 1 = No, 2 = Yes, create a NEWVAR with 1 = Yes, 0 = No using **NEWVAR = OLDVAR - 1**.
    - I would treat the `RIAGENDR` variable as describing biological sex and would rename it as I created a factor.
    - The family income ratio `INDFMPIR` is appealing and quantitative, but it has a pronounced ceiling effect. It is the ratio of income to the poverty level, but is capped at 5. How should you think about that? 
        - A similar issue applies to several other variables, including age (in adults) which are capped at 80.
    - When working with the education `DMDEDUC2` variable or others with many categories, collapse levels sensibly.
5. Advice that applies to everyone's Study 2, even if you're not using NHANES include:
    - You cannot use the same variable (or any form of the same underlying variable) as both an outcome and a predictor.
    - Variables that use categories to describe what were originally quantitative variables aren't quantitative any more.
    - Things I would treat as missing include Refused, Don't Know, Unknown, No response and missing. Be sure that R recognizes things that are missing as missing and filters them out when you filter for complete cases.
    - You are allowed (not encouraged, just allowed) to impute things other than your outcome or key predictor, if you want to, but it won't help if you don't do it correctly. You are not allowed in Project B to impute your outcome or key predictor.
6. [Data is Plural](https://tinyletter.com/data-is-plural) is a nice (and free) weekly newsletter of useful/curious data sets curated by Jeremy Singer-Vine. You might be interested in taking a look.
7. [The Daily](https://thedaily.case.edu/tell-us-what-youre-thankful-for-this-year/) is interested to hear from you about what you're thankful for this year. 
    - I'm thankful for your patience with me, and especially thankful for the **incredible** support we've all received from our teaching assistants.
8. No class next week. Our next class is Tuesday 2020-12-01. 
    - TA office hours will be held through Friday 2020-11-20 and then not again until Saturday 2020-11-28. 
    - Dr. Love will address Piazza questions and emails on Monday 2020-11-23 and then not again regularly (although he'll check in when he can) until Monday 2020-11-30.
9. All business regarding 431 will be concluded on 2020-12-14. 
    - Dr. Love will be out of the office from 2020-12-15 through 2021-01-03, and will be less responsive in January to email than usual. 
    - 432 begins at the start of February, and all students successfully completing 431 with a grade of A or B will be cheerfully welcomed to 432.

## What Should I Be Working On?

1. Staying healthy, keeping other people healthy, and taking care of those that need your help. **Make good choices.**
2. Your Project B [Study 2 Data Plan](https://thomaselove.github.io/431-2020-projectB/your5.html), if not already approved.
3. Over the break, please:
    - finish reading Spiegelhalter's *The Art of Statistics*
    - watch the [extra videos from Class 20](https://github.com/THOMASELOVE/431-2020/tree/master/classes/class20#the-extra-materials-for-class-20-are-provided-below)
4. [Lab 8](https://github.com/THOMASELOVE/431-2020/blob/master/labs/lab08/lab08.md) is due Monday 2020-11-30.
5. [Project B](https://thomaselove.github.io/431-2020-projectB) Study 1 and Study 2 are now in your hands, assuming I've approved your Data Plan. The reports and other materials are due 2020-12-10 at noon.

## One Last Thing

There was a very important piece published this week that I expect you all might benefit from reading.

- It's called [Five rules for evidence communication](https://www.nature.com/articles/d41586-020-03189-1) by Michael Blastland, Alexandra L.J. Freeman, Sander van der Linden, Theresa M. Marteau and *David Spiegelhalter* and it's a comment published in *Nature* 2020-11-19. 
    - Here's a [PDF of the main comment](https://github.com/THOMASELOVE/431-2020/blob/master/classes/class24/pdf/nature_five_rules_for_evidence_communication_2020.pdf) (3 pages).
    - Here's a [PDF of the supplemental information](https://github.com/THOMASELOVE/431-2020/blob/master/classes/class24/pdf/nature_supplemental_information_2020.pdf) which details the arguments further (10 pages).

## COVID Vaccine Trial Protocols (if you're interested)

- [Pfizer protocol is here](https://pfe-pfizercom-d8-prod.s3.amazonaws.com/2020-11/C4591001_Clinical_Protocol_Nov2020.pdf) (PDF).
- [Moderna protocol is here](https://www.modernatx.com/sites/default/files/mRNA-1273-P301-Protocol.pdf) (PDF).

from STAT News: [Pfizer and BioNTech to submit Covid-19 vaccine data to FDA as full results show 95% efficacy](https://www.statnews.com/2020/11/18/pfizer-biontech-covid19-vaccine-fda-data) by Damian Garde and Matthew Herper, 2020-11-18.

> Of the 170 cases of Covid-19 that were recorded from the trial, 162 were in the placebo arm, while the rest were among those who got two doses of the Covid-19 vaccine. Ten of the infections overall were severe — nine of which were in the placebo group.

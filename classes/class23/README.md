# 431 Class 23: 2020-11-17

[Main Website](https://thomaselove.github.io/431/) | [Course Calendar](https://thomaselove.github.io/431/calendar.html) | [Syllabus](https://thomaselove.github.io/431-2020-syllabus/) | [Course Notes](https://thomaselove.github.io/431-notes/) | [Piazza & TA Office Hours](https://thomaselove.github.io/431/contact.html) | [Canvas](https://canvas.case.edu) | [Data and Code](https://thomaselove.github.io/431/data_index.html)
:-----------: | :--------------: | :----------: | :---------: | :-------------: | :-----------: | :------------:
for everything | for deadlines | expectations | from Dr. Love | ways to get help | zoom information | for downloads

![](https://github.com/THOMASELOVE/431-2020/blob/master/classes/class23/images/senn_personal.PNG)

## Today's Slides

- Class 23 slides are available in [PDF format](https://github.com/THOMASELOVE/431-2020/blob/master/classes/class23/431_class-23-slides_2020.pdf), as well as in [R Markdown](https://github.com/THOMASELOVE/431-2020/blob/master/classes/class23/431_class-23-slides_2020.Rmd).
  - Remember that these are actually slides for Classes 22-24.

## Announcements

1. The Lab 07 sketch and rubric **will be posted** on Tuesday 2020-11-17 by noon.
2. Grades on Lab 06 are [now posted](http://bit.ly/431-2020-grades) in the usual place. 
    - Here's a [reminder regarding Regrade Requests](https://github.com/THOMASELOVE/431-2020/tree/master/labs#grading-errors-and-regrade-requests).
    - Here's a [reminder about our policy on late Lab assignments](https://github.com/THOMASELOVE/431-2020/tree/master/labs#late-work).
3. Project A Results
    - Grades and feedback on Project A were emailed on Friday 2020-11-13. If you didn't get your results, please contact Dr. Love. For Project B, you will get much less feedback - no more than your Project B grade, really.
    - I also sent email 2020-11-13 indicating whether you are welcome to work alone or with a partner on Project B (most people) or whether you need to work alone. Let Dr. Love know if you are unclear on your status.
    - I posted detailed [evaluation results, including an example of a good video from Project A](https://github.com/THOMASELOVE/431-2020/blob/master/projects/projectA/evaluation_results.md) that I hope you will look at.
    - In that material, I provided (unedited) responses to two of the questions from the self-evaluation, specifically (1) [What was the key finding of your study](https://github.com/THOMASELOVE/431-2020/blob/master/projects/projectA/evaluation_results.md#what-was-the-key-finding-of-your-study)? and (2) [What is the most important thing that you know now that you wished you'd known when you began Project A](https://github.com/THOMASELOVE/431-2020/blob/master/projects/projectA/evaluation_results.md#what-is-the-most-important-thing-that-you-know-now-that-you-wished-youd-known-when-you-began-project-a)? Perhaps you will find these interesting.
4. Some advice for Project B (some of these happened a lot in Project A) that I've enhanced on the Report Specifications pages for [Study 1](https://thomaselove.github.io/431-2020-projectB/survey5.html) and [Study 2](https://thomaselove.github.io/431-2020-projectB/your6.html).
    1. **YAML** Your YAML should include `code_folding: show` and `r Sys.Date()` and `number_sections: TRUE`.
        - Look at the Project B Study 1 Demo ([view HTML](https://rpubs.com/TELOVE/projB-study1-demo)) ([download Rmd](https://github.com/THOMASELOVE/431-2020/blob/master/projects/projectB/431-projectB-study1-demo.Rmd)) to see each of these elements in action.
    2. **Use my headings** Please use the headings I provided for you in the report specifications, both for [Project B Study 1](https://thomaselove.github.io/431-2020-projectB/survey5.html) and for [Project B Study 2](https://thomaselove.github.io/431-2020-projectB/your5.html), rather than creating new headings of your own. This will help me find what I need more quickly. Save your creativity for what goes under the headings, in particular your visualizations and descriptions of results. 
    3. **No warnings** Your final HTML document should not display any warning messages, not because you've hidden them with `warning = FALSE` but because you've eliminated the need for R to generate them. Don't use `echo = FALSE` or `warning = FALSE` or `include = FALSE` anywhere in the document.
    4. **Avoid useless messages** Your final HTML document should have none of the unnecessary messages that R packages (like mosaic and dplyr) generate. It may be helpful to use `library(mosaic)` to avoid some of them, and you'll want to use `message = FALSE` as needed to remove these from the final product.
    5. **Changing Variable Names** If you change the name of a variable (in either Study 1 or Study 2) from what you initially downloaded, using something other than clean_names(), I'm OK with that (despite my initial response on Piazza to question @339), but you **must do this** before you present your codebook at the end of Section 3 (Cleaning the Data) for each study, and each of your codebooks (one for Study 1, one for Study 2) should include the names I should remember when looking at your analyses. 
        - In Study 1 (and in Study 2 if you're using NHANES) please include the original variable name as part of your codebook at the end of section 3 of your report.
    6. **Dealing with Don't Know** If you're using NHANES (or any other) data for Study 2 that uses "don't know" or "unknown" or "did not respond" as a possible response for a variable, treat those values as missing.
5. In response to a Piazza question (@347), I provided lots of links to information about the NHANES 2017-18 data. If you're planning to use that data, you should be looking at those links.
    - In particular, look at the Doc file (next to the Data file) for each of the groups of variables you are considering (Demographics, Dietary, Examination, Laboratory or Questionnaire.) 
        - For instance, [here is the 2017-18 Demographics page with links to the Doc and the Data](https://wwwn.cdc.gov/nchs/nhanes/search/datapage.aspx?Component=Demographics&CycleBeginYear=2017), and [here's the Doc file](https://wwwn.cdc.gov/Nchs/Nhanes/2017-2018/DEMO_J.htm) on Demographics in 2017-18.
6. Project B oral presentations
    - Dr. Love will provide further details on the oral presentations for Project B on December 1.
    - Some of you will be required to present more extensively, via a 15-20 minute Zoom call, while the rest will present via a pre-recorded video with a strict (and short) time limit answering questions I will pose on December 1.
    - If you are required to give a Zoom presentation, the available times will be on December 9, 10 and 11, and I will do what I can to accommodate your preferences and schedules.
6. Need to pull the coefficients from a regression equation out of an R model to present the equation? Davis Weaver was good enough to suggest the [equatiomatic package](https://github.com/datalorax/equatiomatic). 
7. This Friday 2020-11-20 from 10 AM to 1 PM is the Virtual Public Health Innovations Conference sponored by the MPH program at CWRU, and open to all. [This pdf flyer](https://github.com/THOMASELOVE/431-2020/blob/master/classes/class23/Fall%202020%20Innovations%20full%20agenda.pdf) has all of the information.
    - Several folks affiliated with this course are part of the virtual poster session, and there are some very interesting talks planned, including opening remarks from Daniel Tisch and Peter Zimmerman on "Explaining the current state of COVID-19: Preparing to Answer your relatives' burning questions around the Thanksgiving Dinner Table." 

## What Should I Be Working On?

### Prior to the Thanksgiving Break

1. There is a [Minute Paper after Class 23](https://bit.ly/431-2020-minute-23), due Wednesday 2020-11-18 at Noon.
    - I am eliciting preferences about Project B oral presentations, but I will not be bound by them.
2. The Project B [Study 2 Data Plan](https://thomaselove.github.io/431-2020-projectB/your5.html) is due at noon on Thursday 2020-11-19. 
    - You have all of the information you need to get your Study 2 data now, [either from NHANES or from a source you identify](https://thomaselove.github.io/431-2020-projectB/your1.html). Once you have the data in R, you can complete the [Data Plan](https://thomaselove.github.io/431-2020-projectB/your5.html). Actually filling out the form shouldn't take more than 15 minutes, at most.
    - Dr. Love is reviewing these submissions daily and responding via email. Status reports [are available here](https://github.com/THOMASELOVE/431-2020/blob/master/projects/projectB/study2-dataplan-status.md).
    - It's important for all of you to get the plan in on time, so I can get them all back to you Thursday, and you can make any necessary changes so that you have an accepted plan by 5 PM Friday 2020-11-20.

### During Thanksgiving Break

- TA office hours will be held as usual on Friday 2020-11-20, and then not again until Saturday 2020-11-28. 
- Dr. Love will review Piazza and respond to all questions on Monday 2020-11-23 and then not again before Saturday 2020-11-28.

1. Please finish reading Spiegelhalter's *The Art of Statistics*. It will play a more substantial role in our conversations for Classes 25-26 and it will also appear on Quiz 2.
2. Please watch the [extra videos associated with Class 20](https://github.com/THOMASELOVE/431-2020/tree/master/classes/class20#the-extra-materials-for-class-20-are-provided-below) before the end of Thanksgiving Break. They will help you with Project B Study 1, and with Quiz 2, at the least.
3. [Lab 8](https://github.com/THOMASELOVE/431-2020/blob/master/labs/lab08/lab08.md) is due Monday 2020-11-30. It uses materials from Classes 19-24.
4. Project B Study 1 (which you can do now) and Study 2 reports and other materials are due 2020-12-10 at noon.
    - You can do some of Study 2 now, and you'll be able to do all of it after (1) I've approved [your Study 2 Data Plan](https://thomaselove.github.io/431-2020-projectB/your5.html) **and** (2) we've completed Class 24.

## One Last Thing

To come.

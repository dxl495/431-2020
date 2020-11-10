# 431 Class 21: 2020-11-10

[Main Website](https://thomaselove.github.io/431/) | [Course Calendar](https://thomaselove.github.io/431/calendar.html) | [Syllabus](https://thomaselove.github.io/431-2020-syllabus/) | [Course Notes](https://thomaselove.github.io/431-notes/) | [Piazza & TA Office Hours](https://thomaselove.github.io/431/contact.html) | [Canvas](https://canvas.case.edu) | [Data and Code](https://thomaselove.github.io/431/data_index.html)
:-----------: | :--------------: | :----------: | :---------: | :-------------: | :-----------: | :------------:
for everything | for deadlines | expectations | from Dr. Love | ways to get help | zoom information | for downloads

**Quote to come.**

## Today's Slides

- Class 21 slides are now available in [PDF format](https://github.com/THOMASELOVE/431-2020/blob/master/classes/class21/431_class-21-slides_2020.pdf), as well as in [R Markdown](https://github.com/THOMASELOVE/431-2020/blob/master/classes/class21/431_class-21-slides_2020.Rmd).

## Announcements

1. [Instructions for Project B](https://thomaselove.github.io/431-2020-projectB/) are now available.
    - The newest item(s) posted there are the materials for the [Study 1 Demonstration Project](https://thomaselove.github.io/431-2020-projectB/survey6.html).
    - I also made a lot of small changes yesterday to the site to help clarify issues regarding the oral presentation element of the project.
    - If you're looking for a partner for Project B, please visit the **Project B Looking for a Partner** document in our Shared Google Drive, which you should also be able to access at https://bit.ly/431-projectB-find-a-partner. 
        - There, you can list your name and email and find the names and emails of people who are looking for partners. If you've asked me for help in this regard, you'll also find your information on the list.
        - I ask only that you remove your name and email once you have found a partner. 
2. On 2020-12-04, the San Francisco chapter of the American Statistical Association is hosting a pair of keynote speakers and a panel discussion on [A Positive Outlook During the Covid Era: how statistics could contribute to a better 2021](http://www.sfasa.org/Dec42020mtg.html). Registration is [free and required](https://www.eventbrite.com/e/2020-sfasa-holiday-celebration-tickets-127577564931), if you are interested.
3. The [ggplot2 book](https://ggplot2-book.org/) by Hadley Wickham, Danielle Navarro, and Thomas Lin Pedersen is ramping up its third edition. If you're looking for a cookbook, though, I'd recommend the [R Graphics Cookbook](https://r-graphics.org/) by Winston Chang.
4. [Explore your activity on Google with R](https://towardsdatascience.com/explore-your-activity-on-google-with-r-how-to-analyze-and-visualize-your-search-history-1fb74e5fb2b6) is an interesting piece posted 2020-11-06 by Saul Beuntello at [Towards Data Science](https://towardsdatascience.com/). 

## What Are the Remaining Deliverables This Semester?

### There are four classes (including today) and four deliverables before Thanksgiving Break (prior to 2020-11-20)

1. The [Class Survey](https://thomaselove.github.io/431-2020-projectB/survey1.html) (used for Project B Study 1 data) is due tomorrow (Wednesday 2020-11-11) at 11 PM. 
    - This replaces the Minute Paper after Class 21 that was originally planned.
    - Once Dr. Love has processed these data and provided them to you, you will be able to do **all** of Project B Study 1.
2. [Lab 07](https://github.com/THOMASELOVE/431-2020/blob/master/labs/README.md) is due at 9 PM on Monday 2020-11-16. 
    - Remember that your lowest two lab grades this semester are ignored, so you can skip two if you did well on the others, although Labs 7 and 8 are an excellent way to build up skills for Quiz 2 and Project B.
3. There will be a Minute Paper after Class 23 due 2020-11-18.
4. The Project B [Study 2 Data Plan](https://thomaselove.github.io/431-2020-projectB/your5.html) is due at noon on Thursday 2020-11-19. Assuming you either have found a partner or don't need one, all you need to do there is: 
    - [select your Study 2 data set](https://thomaselove.github.io/431-2020-projectB/your1.html) (either [NHANES](https://thomaselove.github.io/431-2020-projectB/your2.html) or something else that meets [my specifications](https://thomaselove.github.io/431-2020-projectB/your3.html)), 
    - get your Study 2 data into R (I provide [detailed NHANES instructions](https://thomaselove.github.io/431-2020-projectB/your2.html)), 
    - [select your outcome, key predictor, and 3-8 additional predictors](https://thomaselove.github.io/431-2020-projectB/your4.html) you're interested in and establish a research question linking the outcome to the key predictor and (perhaps) the additional predictors,
    - complete some very basic summaries in R (really, just counts of how many "complete" cases you have)
    - fill out the form at http://bit.ly/431-projectB-data-plan ([the questions on the form](https://thomaselove.github.io/431-2020-projectB/your5.html) are available for you to review so you can prepare.)

### After Thanksgiving Break, we have two classes and five deliverables.

5. Watch the five extra videos associated with Class 20, that you'll find in the **Class 20 Extra Videos** folder in our Shared Google Drive, before we return from Thanksgiving Break on 2020-11-30. Somehow, I'll know if you have done this. Hint, hint.
6. [Lab 08](https://github.com/THOMASELOVE/431-2020/blob/master/labs/README.md) is due at 9 PM on Monday 2020-11-30. 
    - Remember that your lowest two lab grades this semester are ignored, so you can skip two if you did well on the others, although Labs 7 and 8 are an excellent way to build up skills for Quiz 2 and Project B.
7. There will be a Minute Paper after Class 25 due 2020-12-02.
8. [Project B] is due 2020-12-10 at Noon.
    - All of you will be submitting your (group's) Study 1 Report (Rmd and HTML) and Study 2 Report (Rmd and HTML).
    - All of you will submit a self-evaluation Google Form that Dr. Love will make available on 2020-12-01.
    - Most of you will submit a video recording of yourself talking about your project in response to questions Dr. Love will provide on 2020-12-01. 
    - Some of you (about 12 project groups in all) will instead meet with Dr. Love via Zoom to discuss Project B either on 2020-12-09, 12-10 or 12-11.
    - You'll know which oral presentation (recording or meeting) you'll need to do by 2020-12-01, when you get the questions.
9. Quiz 2 will be made available to you by 5 PM on Friday 2020-12-04, the day after our last class. It was originally supposed to be due on 2020-12-08, but I've now moved that deadline back to Friday 2020-12-11 at noon.

# One Last Thing

To come.

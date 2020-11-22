# 431 Class 25: 2020-12-01

[Main Website](https://thomaselove.github.io/431/) | [Course Calendar](https://thomaselove.github.io/431/calendar.html) | [Syllabus](https://thomaselove.github.io/431-2020-syllabus/) | [Course Notes](https://thomaselove.github.io/431-notes/) | [Piazza & TA Office Hours](https://thomaselove.github.io/431/contact.html) | [Canvas](https://canvas.case.edu) | [Data and Code](https://thomaselove.github.io/431/data_index.html)
:-----------: | :--------------: | :----------: | :---------: | :-------------: | :-----------: | :------------:
for everything | for deadlines | expectations | from Dr. Love | ways to get help | zoom information | for downloads

**Quote to come**

## Today's Slides

- Class 25 slides will be made available in [PDF format](https://github.com/THOMASELOVE/431-2020/blob/master/classes/class25/431_class-25-slides_2020.pdf), as well as in [R Markdown](https://github.com/THOMASELOVE/431-2020/blob/master/classes/class25/431_class-25-slides_2020.Rmd).

## Changes to Course Materials Since We Last Met

1. [Project B instructions](https://thomaselove.github.io/431-2020-projectB/)
    - In the [Study 2 Report Specifications](https://thomaselove.github.io/431-2020-projectB/your6.html), I added details in sections 3 and 5 which pull together advice I have provided elsewhere plus new information on cleaning data, the codebook, and what to check in your data. I attempted in section 5, in particular, to provide clear **recipes that you should follow** for this critical section of your Study 2 report. 
        - Some of this advice also appeared in the [Class 24 README](https://github.com/THOMASELOVE/431-2020/tree/master/classes/class24). 
        - I also placed a short note at the start of Sections 3 and 5 of the [Study 2 Demonstration Project](https://thomaselove.github.io/431-2020-projectB/your7.html) to remind you to look at these augmented instructions.
2. [Course Notes](https://thomaselove.github.io/431-notes/)
    - Some of this material is a little less up to date than I wish it was. The class slides always show my most recent thinking for R coding, but I haven't found the time to fix that in the Notes in some spots. Newly posted materials include:
    - [Chapter 23](https://thomaselove.github.io/431-notes/estimating-a-population-proportion.html): Building Confidence Intervals for a Population Proportion `posted 2020-11-21`
    - [Chapter 24](https://thomaselove.github.io/431-notes/comparing-proportions-with-two-independent-samples.html): Analyzing a Two-by-Two table to compare proportions `posted 2020-11-21`.
    - [Chapter 25](https://thomaselove.github.io/431-notes/larger-contingency-tables.html): Chi-square tests for larger two-way tables and Cochran-Mantel-Haenszel for three-way tables `posted 2020-11-21`.
    - [Chapter 26](https://thomaselove.github.io/431-notes/power-and-proportions.html): Sample Size and Power when comparing Two Proportions `posted 2020-11-21`.
    - [Chapter 27](https://thomaselove.github.io/431-notes/quiz-2-review.html): Some Practice Problems for Quiz 2 (with solutions) `posted 2020-11-21`.
    - [Chapter 28](https://thomaselove.github.io/431-notes/missing-data-mechanisms-and-simple-imputation.html): Missing Data and Simple Imputation `posted 2020-11-22`.
    - [Chapter 29](https://thomaselove.github.io/431-notes/multiple-regression-introduction.html): Setting Up Multiple Regression Case Studies, Outline of Key 431 Concepts `posted 2020-11-22`.
    - The final chapters (which I will post by 2020-12-01) amplify and augment the regression ideas discussed in Classes 22-24.
3. On Canvas, you should now be able to **download all of our class Zoom recordings**.
    - When logged into 431 on Canvas, click Zoom, then select Cloud Recordings, pull up a recording of a class as if you were watching it, and at the top right, you should find a button to download the recording. I'm sorry it took until now for these to be downloadable.
    - The Zoom videos will start disappearing in mid-January of 2021, so I encourage you to grab them in December if you want them. 
    - 431 Course Notes and Github materials will disappear in early June of 2021, so you have more time to grab them if you like.

## Oral Presentations for Project B

There are three groups of students. You should have received an email from Dr. Love on 2020-11-21 specifying your group. If you are not clear on which group, you're in, let him know via email now.

1. A dozen students who are required to present Project B via a Zoom call with Dr. Love on 2020-12-09, 12-10 or 12-11.
    - These students need to fill out the Google Form I sent to them so I can schedule the Zoom calls. These are the 12 students in the MS program in Health Care Analytics, or the PhD program in PQHS.
2. Two dozen students invited by Dr. Love to present Project B via a Zoom call, but can opt instead to do a recorded video.
    - These students can opt to present via Zoom (in which case they need to fill out the Google Form I sent to schedule their Zoom call) or opt to present via recorded video (in which case they need to email me.)
    - These students included most of the students who preferred to present via Zoom (assuming their partner wasn't against the idea), plus some specific students I wanted to hear from, if possible. 
3. The remaining students, who will be doing a recorded video.
    - This includes students in other time zones, those who didn't want to do a Zoom call (or who had a partner who didn't) as well as some of the prople who were willing to do either, mostly. If you're in this group and really want to present via Zoom, please email me now.

## Announcements

1. **To be posted**. There will be a Minute Paper after Class 25, due at noon Wednesday 2020-12-02. 
2. [The `forcats` package](https://forcats.tidyverse.org/index.html) is an incredibly useful tool for working with factors, but it's sometimes a challenge to figure out which function to use in a particular situation. 
    - [Here is a comprehensive list](https://forcats.tidyverse.org/reference/index.html) of all of the functions available for changing the order of levels, changing the value of level, adding or removing levels, combining multiple factors, and other helper functions, including links to examples.
    - The [RStudio Cheat Sheet (pdf)](https://github.com/rstudio/cheatsheets/raw/master/factors.pdf) for working with factors using `forcats` is very useful.
    - Emily Robinson provides a gentle [introduction to forcats](https://forcats.tidyverse.org/articles/forcats.html)
    - R for Data Science has a [chapter on factors](https://r4ds.had.co.nz/factors.html)
    - Amelia McNamara and Nicholas Horton have a 2017 paper on [Wrangling categorical data in R](https://peerj.com/preprints/3163/) that helped motivate the `forcats` package.
3. **Do I need to upgrade R or RStudio?** 
    - There is no need for you to upgrade until after you complete both Project B and Quiz 2. We assume you have version 4.0.2 of R and RStudio version 1.3.xxx. You are *welcome* to upgrade, but it is more likely to cause problems than solve them for you at this point.
    - Dr. Love intends to continue using R version 4.0.2 and RStudio version 1.3.1056 through the end of the course.
    - As of 2020-11-22, the current versions that are available are R version 4.0.3 and RStudio version 1.3.1093.

# 431 Class 22: 2020-11-12

[Main Website](https://thomaselove.github.io/431/) | [Course Calendar](https://thomaselove.github.io/431/calendar.html) | [Syllabus](https://thomaselove.github.io/431-2020-syllabus/) | [Course Notes](https://thomaselove.github.io/431-notes/) | [Piazza & TA Office Hours](https://thomaselove.github.io/431/contact.html) | [Canvas](https://canvas.case.edu) | [Data and Code](https://thomaselove.github.io/431/data_index.html)
:-----------: | :--------------: | :----------: | :---------: | :-------------: | :-----------: | :------------:
for everything | for deadlines | expectations | from Dr. Love | ways to get help | zoom information | for downloads

![](https://github.com/THOMASELOVE/431-2020/blob/master/classes/class22/images/dataviz.png)

## Today's Slides

- Class 22 slides are now available in [PDF format](https://github.com/THOMASELOVE/431-2020/blob/master/classes/class22/431_class-22-slides_2020.pdf), as well as in [R Markdown](https://github.com/THOMASELOVE/431-2020/blob/master/classes/class22/431_class-22-slides_2020.Rmd).
    - Actually, the slides posted here are longer than usual. They include materials for Classes 22, 23 and 24, so you'll find them posted to those classes as well, as we go along. 
    - The only changes (other than correcting mistakes) I intend to make are adding a slide to indicate where we stopped at the end of class.
    - Over these next three classes, I will discuss everything I am hoping you will use in Project B Study 2 that we have not yet covered, so that you'll be ready to do Study 2 a week from now, once I've signed off on your Study 2 Data Plan.

## Announcements

1. I changed the [Lab 8 instructions](https://github.com/THOMASELOVE/431-2020/blob/master/labs/lab08/lab08.md) to use `slice_sample()` to select the training sample in the leadup to Question 4, so that what you do in Lab 8 will be a better match to what I am looking for you to do in Project B (and in general.)
2. Data for Study 1 in Project B is [now available for both 2019 and 2020](https://thomaselove.github.io/431-2020-projectB/survey3.html), and the Study 1 instructions now reflect the change. [Go here](https://thomaselove.github.io/431-2020-projectB/survey3.html) for information on obtaining the data. 
3. In class, I'll give you an update on Grades for Project A.

## What Should I be working on?

1. Now that the Class Survey is complete and Dr. Love has made the 2019 and 2020 data available for [Study 1 in Project B](https://thomaselove.github.io/431-2020-projectB/survey1.html), you have everything you'll need to complete Study 1 for Project B.
2. [Lab 07](https://github.com/THOMASELOVE/431-2020/blob/master/labs/README.md) is due at 9 PM on Monday 2020-11-16. 
    - Remember that your lowest two lab grades this semester are ignored, so you can skip two if you did well on the others, although Labs 7 and 8 are an excellent way to build up skills for Quiz 2 and Project B.
3. The Project B [Study 2 Data Plan](https://thomaselove.github.io/431-2020-projectB/your5.html) is due at noon on Thursday 2020-11-19.
4. Watch the [extra videos associated with Class 20](https://github.com/THOMASELOVE/431-2020/tree/master/classes/class20#the-extra-materials-for-class-20-are-provided-below) before the end of Thanksgiving Break. I'll know if you did, and they will help with Project B Study 1. Hint, hint.
5. Look at the [Calendar](https://thomaselove.github.io/431/calendar.html) (also summarized in the [Class 21 README](https://github.com/THOMASELOVE/431-2020/tree/master/classes/class21#there-are-ten-remaining-deliverables-this-semester)) for remaining deliverables and deadlines.

![](https://github.com/THOMASELOVE/431-2020/blob/master/classes/class22/images/senn.PNG)

# A Few Things about the Election

- [The Polls Weren’t Great. But That’s Pretty Normal](https://fivethirtyeight.com/features/the-polls-werent-great-but-thats-pretty-normal/) from Nate Silver posted 2020-11-11 at FiveThirtyEight.
- [Lying with Statistics](https://statmodeling.stat.columbia.edu/2020/11/10/lying-with-statistics/) from Andrew Gelman at his blog, 2020-11-10.
- [Where We Saw Red And Blue Mirages On Election Night](https://fivethirtyeight.com/features/where-we-saw-red-and-blue-mirages-on-election-night/) by Laura Bronner, Anna Wiederkehr and Nathaniel Rakich at FiveThirtyEight has a really interesting visualization, copied below.

![](https://github.com/THOMASELOVE/431-2020/blob/master/classes/class22/images/crawl.png)

# One Last Thing

- There's an entertaining video on YouTube entitled [Why do Biden's votes not follow Benford's Law?](https://www.youtube.com/watch?v=etx0k1nLn78) by Matt Parker, who goes by [Stand-up Maths](http://standupmaths.com/) online and has a book out called *Humble Pi* which I hope to get around to reading soon.
- More on [Benford's Law](https://en.wikipedia.org/wiki/Benford%27s_law) like most things, can be found at [Wikipedia](https://en.wikipedia.org/wiki/Benford%27s_law).

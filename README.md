# CS423 Probabilistic Programming, Spring 2020, KAIST

This is a webpage of the course "CS423 Probabilistic Programming", which is offered at the KAIST CS department in the spring of 2020. The webpage will contain links to lecture slides and other course-related materials.

Probabilistic programming refers to the idea of developing a programming language for writing and reasoning about probabilistic models from machine learning and statistics. Such a language comes with the implementation of several generic inference algorithms that answer various queries about the models written in the language, such as posterior inference and marginalisation. By providing these algorithms, a probabilistic programming language enables data scientists to focus on designing good models based on their domain knowledge, instead of building effective inference engines for their models, a task that typically requires expertise in machine learning, statistics and systems. Even experts in machine learning and statistics may get benefited from such a probabilistic programming system because using the system they can easily explore highly advanced models.

This course has two goals. The first is to help students to be a good user of an expressive probabilistic programming language.  Throughout the course, we will use a particular language, called [Anglican](http://probprog.ml/anglican/), but we will emphasise general principles that apply to a wide range of existing probabilistic programming systems. The second goal is to expose the students to recent exciting results in probabilistic programming, which come from machine learning, statistics, programming languages, and probability theory.

## 1. Important Announcements

#### [March 28] [Homework1](https://github.com/hongseok-yang/probprog20/blob/master/Homework/Homework1/homework1-questions.pdf) is out.

The homework assignment 1 is out. Submit your solutions in KLMS by 6:00pm on 8 April 2020 (Wednesday). 

We remind the students that we adopt a very strict policy for handling dishonest behaviours. If a student is found to copy answers from peers or other sources in her or his submission for this homework assignment, he or she will get F.

Best wishes, Hongseok

#### [March 14] Penality scheme for late homework submissions.

Here is our scheme for handling late homework submissions. It assumes that
the total marks are 100.

1. <= One day late: -10
2. <= Two days late: -20
3. <= Three days late: -30
4. <= Four days late: -40
5. More than four days late: -100.

#### [March 14] Project group.

The group project is an important part of this course. Find your project partners by 30 March 2020 (Monday), and inform all of Hongseok, Daeseok, and Kwonsoo by email by the midnight of 30 March 2020. Each group should consist of 1-3 students. (We allow a group of one student because of the special circumstance of moving a large amount of course activities online this year.)

#### [March 8] Honour code.

The course will adopt very strict honour code. If a student is found to copy homework solutions from friends and other sources, he or she will get F. Similarly, if a student is found to do cheaing during exam, she or he will get F as well. 

#### [March 8] Online lectures for the first two weeks at least.

Because of Covid-19, the lectures for the first two weeks at least (16 March 2020 - 27 March 2020) will be held online at the usual schedule. We will use ZOOM, and you should have received information about how to access it from the university and the department. The access keys to online sessions will be provided in KLMS. 

Another measure that we take is not to have any face-to-face meetings between teaching staffs and students, again because of Covid-19. This means that offline office hours won't be held for a while. To get help, please use the discussion forums in KLMS.

## 2. Logistics

#### Evaluation

* Final exam (40%). Project (40%). Homework (20%).

#### Teaching Staffs

* Lecturer: [Prof Hongseok Yang](https://cs.kaist.ac.kr/people/view?idx=552&kind=faculty&menu=160) (email: hongseok00@gmail.com, office hours: 6:00pm - 7:00pm on Monday in ZOOM. You can find more information about it in KLMS.)
* TA1: Gwonsoo Che (email: gwonsoo.che@gmail.com, office hours: 6:00pm - 7:00pm every other Thursday through ZOOM. See KLMS announcements for more information.)
* TA2: Daeseok Lee (email: daeseoklee@kaist.ac.kr, office hours: 7:30pm - 8:30pm every other Thursday through ZOOM. See KLMS announcements for more information.)

#### Place and Time

* Place: room 111 in the N1 building
* Time: 1:00pm - 2:15pm on Monday and Wednesday from 16 March 2020 until 29 June 2020. For the first weeks and possibly more, we will have virtual online classes using ZOOM.
* Final exam: 1:00pm - 3:00pm on 10 June 2019 (Monday) at the room 111 in the N1 building.

#### Online Discussion

* We will use KLMS.

## 3. Homework

Submit your solutions in KLMS. We will create submission folders for all the homework assignments in KLMS.

* [Homework0](https://github.com/hongseok-yang/probprog20/blob/master/Homework/Homework0/homework0.pdf) - Don't submit.
* [Homework1](https://github.com/hongseok-yang/probprog20/blob/master/Homework/Homework1/homework1-questions.pdf) - Deadline: 6:00pm on 8 April 2020.

## 4. Tentative Plan

* 03/16 (Mon) - Introduction. [Slides](https://github.com/hongseok-yang/probprog20/blob/master/Lectures/Lecture1/Lecture1.pdf). [Homework0](https://github.com/hongseok-yang/probprog20/blob/master/Homework/Homework0/homework0.pdf). [Gorilla worksheet](https://github.com/hongseok-yang/probprog20/blob/master/Homework/Homework0/linear.clj)
* 03/18 (Wed) - Basics of Clojure and Tiny Bit of Anglican. [Slides](https://github.com/hongseok-yang/probprog20/blob/master/Lectures/Lecture2/Lecture2.pdf). [Gorilla worksheet](https://github.com/hongseok-yang/probprog20/blob/master/Lectures/Lecture2/RandomFibLec2.clj). [Programs](https://github.com/hongseok-yang/probprog20/blob/master/Lectures/Lecture2/).
* 03/23 (Mon) - Basics of Clojure and Tiny Bit of Anglican.
* 03/25 (Wed) - Posterior Inference, Basics of Anglican, and Importance Sampling. [Slides](https://github.com/hongseok-yang/probprog20/blob/master/Lectures/Lecture3/Lecture3.pdf). 
* 03/30 (Mon) - Posterior Inference, Basics of Anglican, and Importance Sampling.
* 04/01 (Wed) - Generative Modelling with Anglican. [Slides](https://github.com/hongseok-yang/probprog20/blob/master/Lectures/Lecture4/Lecture4.pdf). [Gorilla worksheet for 2D physics](https://github.com/hongseok-yang/probprog20/blob/master/Lectures/Lecture4/lecture4_physics.clj). [Gorilla worksheet for program induction](https://github.com/hongseok-yang/probprog20/blob/master/Lectures/Lecture4/lecture4_progind.clj). (Note: In order to run the 2D physics example, you will have to copy [bounce.clj](https://github.com/hongseok-yang/probprog20/blob/master/Lectures/Lecture4/bounce.clj) to the anglican-user/src directory and replace anglican-user/project.clj by [this file](https://github.com/hongseok-yang/probprog20/blob/master/Lectures/Lecture4/project.clj)).
* 04/06 (Mon) - Markov Chain Monte Carlo. [Slides](https://github.com/hongseok-yang/probprog20/blob/master/Lectures/Lecture5/Lecture5.pdf). 
* 04/08 (Wed) - Markov Chain Monte Carlo.
* 04/13 (Mon) - Markov Chain Monte Carlo.
* __**04/15 (Wed) - NO LECTURE. Election Day.**__
* 04/20 (Mon) - Advanced Topic on Markov Chain Monte Carlo.
* 04/22 (Wed) - Advanced Topic on Markov Chain Monte Carlo.
* 04/27 (Mon) - Group Project Pitch.
* 04/29 (Wed) - Advanced Topic on Importance Sampling.
* __**05/04 (Mon), 05/06 (Wed) - NO LECTURES. Midterm Exam.**__
* 05/11 (Mon) - Implementing Inference Algorithms for Probabilistic Programs.
* 05/13 (Wed) - Implementing Inference Algorithms for Probabilistic Programs.
* 05/18 (Mon) - Implementing Inference Algorithms for Probabilistic Programs.
* __**05/20 (Wed) - NO LECTURE. Graduate Admission.**__
* 05/25 (Mon) - Stochastic Variational Inference. 
* 05/27 (Wed) - Stochastic Variational Inference.
* 06/01 (Mon) - Amortised Inference. 
* 06/03 (Wed) - Advanced Topic on Variational Inference and Model Learning.
* 06/08 (Mon) - Denotational Semantics of Probabilistic Programs.
* 06/10 (Wed) - Denotational Semantics of Probabilistic Programs.
* 06/15 (Mon) - Denotational Semantics of Probabilistic Programs.
* 06/17 (Wed) - Student Presentation.
* 06/22 (Mon) - Student Presentation.
* 06/24 (Wed) - Student Presentation.
* __**06/29 (Mon), 07/01 (Wed) - NO LECTURES. Final Exam.**__

## 5. Studying Materials

Studying the lecture slides and notes and the homework exercises of the course is likely to be the most time-efficient way to catch up with this course. Also, at each lecture, we will give students pointers to the related papers. If a student does not understand a certain concept, we encourage him or her to look it up in the Internet. We typically do this when we encounter a similar problem. In our case, Wikipedia, lecture notes or survey articles have helped us the most.

The next best option is to read the following draft book on probabilistic programming:

1. "[An Introduction to Probabilistic Programming](https://arxiv.org/abs/1809.10756)" by Jan-Willem van de Meent, Brooks Paige, Hongseok Yang and Frank Wood. Reading this book will give a broader view on probabilistic programming and much deeper understanding into its inference algorithms and their implementations.

If a student feels that she or he lacks background knowledge on machine learning, we recommend him or her to have a look at the following online materials.

2. The online book "[Probabilistic Programming and Bayesian Methods for Hackers](https://github.com/CamDavidsonPilon/Probabilistic-Programming-and-Bayesian-Methods-for-Hackers)" describes Bayesian Machine Learning using a probabilistic programming system called PyMC. Hongseok found this book easy to follow and good at explaining basics and intuitions.

3. A more standard reference on machine learning is Bishop's book "Pattern Recognition and Machine Learning".

Two good ways to understand probabilistic programming are to try a wide range of examples and to understand common implementation techniques for probabilistic programming languages. The following documents provide such examples or explain those techniques.

4. [Anglican website](https://probprog.github.io/anglican/index.html). In particular, students will learn a lot by trying examples in the site.

5. [Forestdb.org](http://forestdb.org/) is a great source of interesting probabilistic programs.

6. [Edward tutorial website](http://edwardlib.org/tutorials/) and [Pyro example website](http://pyro.ai/examples/). Edward and Pyro are so called deep probabilistic programming languages that attempt to combine deep learning and probabilistic programming. These web pages contain interesting examples that one can try using these languages.

7. Goodman and Stuhlmuller's book "[The Design and Implementation of Probabilistic Programming Languages](http://dippl.org/)". This web-based book describes the implementation of [WebPPL](http://webppl.org/), a probabilistic programming language on top of JavaScript. Many techniques in the book are general and apply to other probabilistic programming languages.

Frank Wood taught a graduate-level course on probabilistic programming at UBC. It emphasises on actually building efficient runtimes for probabilistic programming languages. Here is a link to his course.

8. Wood's [graduate-level course](https://www.cs.ubc.ca/~fwood/CS532W-539W/) at UBC.

## 6. Group Project

1. Kwangjo Gong, Donghyeon Kim, Suho Yang
2. Herin Park, Hyojin Shim
3. Eunseob Kim, Sumin Shin
4. Taeyoung Kim, Janggun Lee, Geon Park
5. Michael Poli
6. Gabin An, Sungmin Kang
7. Jaemin Kim, Yunseok Lee
8. Tung Duong Mai, Assem Zhunis
9. Taehyouk Cho
10. Euicheon Lee, Hyunjae Lee
11. Hongchan An
12. Yujin Nam
13. Dongjoon Yun
14. Euojin Kim
15. Daeseok Lee
16. Dongyeun Lee
17. Seokin Seo, Jinu Choi, Juhyung Park

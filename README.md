# EPFL CS-522: Principles of Computer Systems

_Last updated: September 30, 2025_


## Description

This course is targeted primarily at students who wish to acquire a deep understanding of computer system design or pursue research in systems. It is an intellectually challenging, fast paced course, in which survival requires a good background in operating systems, computer architecture, databases, networking, and programming languages.

A modern computer system spans many layers &ndash; applications, libraries, operating systems, networks, and hardware devices &ndash; with the boundaries between these layers being sometimes fuzzy. Building a good system entails making the right trade-offs (e.g., between performance, durability, and correctness) and understanding emergent behaviors &ndash; the difference between great system designers and average ones is that the really good ones make these trade-offs in a principled fashion, not by trial-and-error. In this course, we identify some of the key principles underlying successful systems, and learn how to solve problems in computing using ideas, techniques, and algorithms from operating systems, networks, databases, programming languages, and computer architecture. The basic courses on these topics teach how the elemental parts of modern systems work; POCS picks up where those courses leave off and focuses on how the pieces come together to form useful, efficient systems.

## Staff

Instructor: [Prof. George Candea](http://dslab.epfl.ch/people/candea)<br>
Co-instructor: [Prof. Katerina Argyraki](http://people.epfl.ch/katerina.argyraki)<br>
TAs: [Can Cebeci](https://dslab.epfl.ch/people/cebeci/) and [Jiacheng Ma](https://dslab.epfl.ch/people/jiacma/)

The staff is reachable at pocs-staff@dslab.org for any private issues you may have; for questions whose answers could benefit other students, please use the [class forum](https://moodle.epfl.ch/mod/lti/view.php?id=1260636).

## Schedule for Fall 2025

We meet twice a week from 11:15&ndash;13:00: Tuesdays in [MA A1 10](https://plan.epfl.ch/?room==MA%20A1%2010) for lectures and Fridays in [PH H3 31](https://plan.epfl.ch/?room==PH%20H3%2031) for recitations.
There are no classes during the week of October 20-25 (Fall break).
We have an exam on Tuesday, December 16.

## Syllabus

| **Week**               | **Lecture** (Tue)                          | **Recitation** (Fri)                                                                                                                                                                                                                                                        | **Quiz** |
|------------------------|-----------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:--------:|
| _Wk1_: Sep 9 + 11     | Modularity &amp; Abstraction [[slides](https://moodle.epfl.ch/pluginfile.php/3465911/mod_folder/content/0/Wk1%20-%20Modularity%20and%20Abstraction.pdf?forcedownload=1)<!-- \| [recitation](https://drive.google.com/file/d/1lRjoVViazl43fOFbPVbb9wX1A1MoFJbB/view?usp=sharing)-->]    | [Exokernel](https://dl.acm.org/doi/pdf/10.1145/224057.224076)<br>>focus on interfaces                                                                                                              | Q1       |
| _Wk2_: Sep 16 + 19     | Naming &amp; Indirection [[slides](https://moodle.epfl.ch/pluginfile.php/3465911/mod_folder/content/0/Wk2%20-%20Naming%20and%20Indirection.pdf?forcedownload=1)] </br><!--  [[slides](lectures/Wk2%20-%20Naming%20&%20Indirection.pdf) \| [lecture notes](https://drive.google.com/file/d/1iDn_p6PWe4ulE7fd-oVxpYibMQzTXo0R/view) \| [recitation](https://drive.google.com/file/d/169TOUhSutedkb_JBlJacVrHFpEgKo6mr/view?usp=sharing)]  --> | [Global Name Service](https://www.cs.princeton.edu/courses/archive/spring13/cos598C/Lampson.pdf)<br>(optionally also [Chord](https://pdos.csail.mit.edu/papers/chord:sigcomm01/chord_sigcomm.pdf)) | Q2       |
| _Wk3_: Sep 23 + 26     | Layering [[slides](https://moodle.epfl.ch/pluginfile.php/3465911/mod_folder/content/0/Wk3%20-%20Layers.pdf?forcedownload=1)] </br><!-- [recitation](https://drive.google.com/file/d/1HyYnSX8wgRKAzMqn55CRrP7nk74gkfhz/view?usp=drive_link)]    -->                     | [RON](https://www.cs.cmu.edu/~dga/papers/ron-sosp2001.pdf)<br>(optionally also [Multi-path TCP](https://www.usenix.org/legacy/events/nsdi11/tech/full_papers/Wischik.pdf))                                                                                   |          |
| _Wk4_: Sep 30 +<br> Oct 3       | Virtualization [[slides](https://moodle.epfl.ch/pluginfile.php/3465911/mod_folder/content/0/Wk4%20-%20Memory%20virtualization.pdf?forcedownload=1)]  <br> Case study: Memory Virtualization         | Case study: Machine Virtualization [[slides PPT](lectures/Wk6%20-%20Machine%20Virtualization.pptx) \| [video](https://youtu.be/Rvp4rnFaYJM)]<br>[Formal requirements for virtualization](https://dl.acm.org/doi/pdf/10.1145/361011.361073)                                                                                                                       |          |
| _Wk5_: Oct 7 + 10      | Case study: DDOS <!-- [[slides](lectures/Wk4%20-%20The%20Internet.pdf)] -->          |  Case study: Modern DNS<br>[Akamai](https://www.akamai.com/site/en/documents/research-paper/akamai-dns-providing-authoritative-answers-to-the-worlds-queries.pdf)                                                                                                                                                | Q3       |
| _Wk6_: Oct 14 + 17     | Technical writing | Writing workshop<br><em>readings TBD</em>                                                                                     |          |
| <center>&mdash;</center> | <center><font color="gray">Fall Break</font></center>           | <center>&mdash;</center>                                                                                                                                                                                                                                     |          |
| _Wk7_: Oct 28 + 31  | Client/Server Organization <!-- [[slides](lectures/Wk7%20-%20Client-Server.pdf) \| [recitation](https://drive.google.com/file/d/1HvB-W5AuYyejKZfyQNhqd983aybU5WRG/view?usp=sharing)]--> | [Microkernel](https://dl.acm.org/doi/pdf/10.1145/224056.224075)<br>>focus on client/server isolation via messages                                                                                                                                            |        |
| _Wk8_: Nov 4 + 7       | Laziness &amp; Speculation <!-- [[video](https://www.youtube.com/playlist?list=PL0kjcN6hElYGhAWhtvQuTO58qNBGZbURH) \| [slides](lectures/Wk8%20-%20Lazy-Speculative.pdf)]   -->      | <em>readings TBD</em>                                                                                                                                                                                                                                         | Q4         |
| _Wk9_: Nov 11 + 14     | Redundancy <!-- [[slides](lectures/Wk10%20-%20Redundancy.pdf) \| [recitation](https://drive.google.com/file/d/1MeXU3yROu_M0QqNwkXX_HhH4LgXkWGlb/view?usp=sharing)]   -->                     | [RAID](https://dl.acm.org/doi/pdf/10.1145/971701.50214) and [RAMcloud](https://dl.acm.org/doi/pdf/10.1145/1713254.1713276)<br>>focus on how redundancy is used                                                                                               |   
| _Wk10_: Nov 18 + 21    | Case study: Transactions <!-- [[video](https://www.youtube.com/watch?v=WnSzmffSFvQ&list=PL0kjcN6hElYF9pp2BzKtBkwgdMsBO3a7g) \| [slides](lectures/Wk11%20-%20Transactions.pdf) \| [recitation](https://drive.google.com/file/d/15lCfmrtytEHzUlwbYkHsYIGXdfTcLI8u/view?usp=sharing)] -->             | [Replication explained through baseball](https://dl.acm.org/doi/pdf/10.1145/2500500) and [CAP 12 yrs later](https://www.infoq.com/articles/cap-twelve-years-later-how-the-rules-have-changed/)<br>>focus on transactional semantics & redundancy             |   Q5   |
| _Wk11_: Nov 25 + 28    | ⚠️<em>Recitation:</em>  [Working set analytics](https://dl.acm.org/doi/10.1145/3399709)   | ⚠️ _Lecture_: Locality &amp; Caching <!-- [[slides](lectures/Wk9%20-%20Locality%20&%20Caching.pdf) \| [recitation](https://drive.google.com/file/d/1mAmqtDMwaeCSXtZvfkQqwort8JHOpG8y/view?usp=sharing)]                      -->                                                                                                                                                                        |
| _Wk12_: Dec 2 + 5      | Hardware/Software Co-Design <!-- [[slides](lectures/Wk12%20-%20Hardware-Software%20Codesign.pdf) \| [recitation](https://drive.google.com/file/d/1hs1V7-VwA2zW9YaWMKwhirmR_-Plt9At/view?usp=sharing)]     -->   | [A new golden age for computer architecture](https://www.youtube.com/watch?v=3LVeEjsn8Ts&t=2183s) <br /> <!-- (about 10 minutes, up to when Patterson starts) <br /> --> and [There's plenty of room at the top](https://www.science.org/doi/10.1126/science.aam9744) | Q6       |
| _Wk13_: Dec 9 + 12    | Exam Review                        | [Past POCS exams](./exams/README.md) + [MCQs](https://drive.google.com/file/d/1NXbngcNrDv4m7igfRjGbo9JPtGRixfnv/view?usp=sharing)                                                                                                                                                              |          |
| _Wk14_: Dec 16 + 19    | Exam on Dec 16 @ 11:15 in lecture room | Exam solution discussion                                                                                                                                                                        |          |

The weekly readings are typically classic Computer Systems papers that embody the principle discussed that week and that have withstood the test of time.

Quizzes take place on the Friday of the week indicated in the syllabus.
They are short, in-class, and handwritten.
A quiz can cover any material covered in the course up to that point.


## Grading 

Your grade for the course will be computed 50% based on the quizzes and 50% based on the exam. 
We will adjust grades in cases where we consider that the computed outcome does not correspond to the student’s mastery of the subject.

## Prerequisites

This course is meant primarily for students who intend to pursue research in the area of systems, therefore you must have a solid systems background. 
Without this background, it is hard to succeed in POCS.
One way to acquire this background is, for example, by taking the following courses (or equivalent):

<!--- 
* CS-323 is not offered this semester and the website for the previous years' website is down. This is a link to an archived PDF-coursebook.
--->

- [CS-477: Advanced operating systems](https://edu.epfl.ch/coursebook/en/advanced-operating-systems-CS-477)
- [COM-407: TCP/IP networking](https://edu.epfl.ch/coursebook/en/tcp-ip-networking-COM-407)
- [CS-470: Advanced computer architecture](https://edu.epfl.ch/coursebook/en/advanced-computer-architecture-CS-470)
- [CS-460: Systems for data management and data science](https://edu.epfl.ch/coursebook/en/systems-for-data-management-and-data-science-CS-460)

If you wish to brave it out despite an incomplete background, be ready to spend at least 2x more time than the other students in order to acquire, on the side, the necessary background on your own.
To compensate for gaps in your background, you can try the textbook [Principles of Computer System Design: An Introduction](https://ocw.mit.edu/resources/res-6-004-principles-of-computer-system-design-an-introduction-spring-2009/) by J. H. Saltzer and M. F. Kaashoek; it’s available in the EPFL library as well as various places online.
We reserve the right to deny enrollment to students who do not fulfill the prerequisites.

## Workload

This course carries 8 ECTS credits.  According to [the EPFL guidelines](https://www.epfl.ch/education/teaching/teaching-guide-2/getting-started/design-a-course_1/#:~:text=A%20full%2Dtime%20student%20is,of%20student%20work%2C%20per%20week), this corresponds to 240 hours of total study time. 
Divided evenly over the 14 weeks of the semester, this leads to an average of a little over 17 hours/week.  This is a big chunk of time in which you can accomplish a lot, as long as you are well organized.

Outside of lectures and recitations, we expect you to spend this time reading the assigned papers multiple times, preparing your critical thoughts and questions on them, thinking deeply about design exercises and producing candidate answers. Doing so will enable you to participate meaningfully in the in-class discussions, ultimately helping you build the skills neccessary to succeed in POCS.

## Attendance Policy

In-person attendance of lectures and recitations is crucial to the learning process.
Attendance by videoconference is not possible.
Some lectures might be recorded, but this is not guaranteed.
Recitations will not be recorded.
The quizzes are given during recitation and are pen-and-paper, so they cannot be taken remotely.

We find that students who do not attend lectures and recitations on a regular basis end up spending much more time studying for the course, and ultimately perform less well.

## Collaboration Policy 

Collaboration and discussion are encouraged via the [class forum](https://moodle.epfl.ch/mod/lti/view.php?id=1260636), visible to the entire class. You can ask questions about the course, the materials, etc. We encourage you to answer questions from your fellow students.

No collaboration is permitted on quizzes or the exam. Cheating, plagiarism, and any form of dishonesty will be handled with the maximum severity permitted under EPFL rules. If you are in doubt whether an action on your part is acceptable, please ask the course staff privately via the staff e-mail list before proceeding. Asking afterward is too late.

## Archived Materials

You can find related materials from previous years below.
Note that the topics covered in the course change from year to year, so archived material might no longer be relevant.

- [How to give a tech talk](talks.md)
- [Final exams](exams/final/README.md)
- [Midterm exams](exams/midterm/README.md)

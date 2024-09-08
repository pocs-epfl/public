# EPFL CS-522: Principles of Computer Systems

<center><strong><font color="red">Draft subject to change</font></strong></center>

## Description

This course is targeted primarily at students who wish to acquire a deep understanding of computer system design or pursue research in systems. It is an intellectually challenging, fast paced course, in which survival requires a good background in operating systems, databases, networking, programming languages, and computer architecture.

A modern computer system spans many layers: applications, libraries, operating systems, networks, and hardware devices. Building a good system entails making the right trade-offs (e.g., between performance, durability, and correctness) and understanding emergent behaviors—the difference between great system designers and average ones is that the really good ones make these trade-offs in a principled fashion, not by trial-and-error. In this course, we identify some of the key principles underlying successful systems, and learn how to solve problems in computing using ideas, techniques, and algorithms from operating systems, networks, databases, programming languages, and computer architecture. The basic courses on these topics teach how the elemental parts of modern systems work; POCS picks up where those courses leave off and focuses on how the pieces come together to form useful, efficient systems.

## Staff

Instructors: [Prof. Katerina Argyraki](http://people.epfl.ch/katerina.argyraki) and [Prof. George Candea](http://dslab.epfl.ch/people/candea)

TAs: [Can Cebeci](http://dslab.epfl.ch/people/cebeci) and [Jiacheng Ma](http://dslab.epfl.ch/people/jiacma)

The staff is reachable at pocs-staff@dslab.org for any private issues you may have; for questions whose answers could benefit other students, please use the class forum (accessed via Moodle).

## Schedule for Fall 2024

We meet twice a week from 11:15&mdash;13:00 in [BC01](https://plan.epfl.ch/?room==BC%2001), except the week of October 21-25 (Fall break).

**Lectures** on Tuesdays, **Recitations** on Fridays

*Exam review*: Tuesday 10-Dec (<font color="red">Friday 13-Dec??</font>)<br>
**Exam**: Tuesday 17-Dec<br>
*Exam discussion*: Friday 20-Dec <br>

## Syllabus

| **Week**               | **Topic**                          | **Readings**             |
|------------------------|------------------------------------|--------------------------|
| _Wk1_: Sep 10 + 13     | Modularity &amp; Abstraction       | [Exokernel](https://dl.acm.org/doi/pdf/10.1145/224057.224076) <br>  (focus on interfaces) |
| _Wk2_: Sep 17 + 20     | Naming &amp; Indirection           | [Global Name Service](https://www.cs.princeton.edu/courses/archive/spring13/cos598C/Lampson.pdf) + [Chord](https://pdos.csail.mit.edu/papers/chord:sigcomm01/chord_sigcomm.pdf) |
| _Wk3_: Sep 24 + 27     | Layering                           | [Multi-path TCP](https://www.usenix.org/legacy/events/nsdi11/tech/full_papers/Wischik.pdf) + [RON](https://www.cs.cmu.edu/~dga/papers/ron-sosp2001.pdf) |
| _Wk4_: Oct 1 + 4       | Case study: The Internet           | [Akamai](https://www.akamai.com/site/en/documents/research-paper/akamai-dns-providing-authoritative-answers-to-the-worlds-queries.pdf)                      |
| _Wk5_: Oct 8 + 11      | Case study: Virtual Memory         | [Twizzler](https://www.usenix.org/system/files/atc20-bittman.pdf) <br> (focus on naming and interfaces to memory) |
| _Wk6_: Oct 15 + 18     | Case study: Machine Virtualization | [Formal reqs for virtualization](https://dl.acm.org/doi/pdf/10.1145/361011.361073) + [Xen](https://dl.acm.org/doi/pdf/10.1145/1165389.945462) <br> (focus on layering and interfaces)  |
| <center>Break</center> | <center>&mdash;</center>           | <center>&mdash;</center> |
| _Wk7_: Oct 29 + Nov 1  | Client/Server Organization         | [Microkernel](https://dl.acm.org/doi/pdf/10.1145/224056.224075) + [Duality of OS structs](https://dl.acm.org/doi/pdf/10.1145/850657.850658) <br> (focus on client/server isolation via messages) |
| _Wk8_: Nov 5 + 8       | Locality &amp; Caching             | [Working Set Analytics](https://dl.acm.org/doi/10.1145/3399709)   |
| _Wk9_: Nov 12 + 15     | Redundancy                         | [RAID](https://dl.acm.org/doi/pdf/10.1145/971701.50214) + [RAMcloud](https://dl.acm.org/doi/pdf/10.1145/1713254.1713276) <br> (focus on how redundancy is used) |
| _Wk10_: Nov 19 + 22    | Case study: Transactions           | [Replication explained through baseball](https://dl.acm.org/doi/pdf/10.1145/2500500) + [CAP 12 yrs later](https://www.infoq.com/articles/cap-twelve-years-later-how-the-rules-have-changed/) <br> (focus on transactional semantics & redundancy)|
| _Wk11_: Nov 26 + 29    | Laziness &amp; Speculation         | Design questions on lazy and speculative execution <br> (No assigned reading) |
| _Wk12_: Dec 3 + 6      | Hardware/Software Co-Design        | [A New Golden Age for Computer Architecture](https://www.youtube.com/watch?v=3LVeEjsn8Ts&t=2183s) <br> (about 10 minutes, up to when Patterson starts) <br>[There’s plenty of room at the Top](https://www.science.org/doi/10.1126/science.aam9744) |
| _Wk13_: Dec 10 + 13    | Exam Review                        | <center>&mdash;</center> |
| _Wk14_: Dec 17 + 20    | Exam                               | <center>&mdash;</center> |


## Grading 

<font color="red">TBD</font>

## Prerequisites

<font color="red">TBD</font>

## Workload

This course carries 8 ECTS credits.  According to [the EPFL guidelines](https://www.epfl.ch/education/teaching/teaching-guide-2/getting-started/design-a-course_1/#:~:text=A%20full%2Dtime%20student%20is,of%20student%20work%2C%20per%20week), this corresponds to 240 hours of total study time. 
Divided evenly over the 14 weeks of the semester, this leads to an average of a bit over 17 hours/week.  This is a big chunk of time in which you can accomplish a lot, as long as you are well organized.

## Attendance Policy

In-person attendance of lectures and recitations is crucial to the learning process.
It is however not mandatory.
Attendance by videoconference is not possible.
Some lectures might be recorded, but this is not guaranteed.

We find that students who do not attend lectures and recitations on a regular basis end up spending much more time studying for the course, and ultimately perform less well.

## Collaboration Policy 

Collaboration and discussion are encouraged via the class forum, visible to the entire class. You can ask questions about the course, the materials, etc. We encourage you to answer questions from your fellow students.

No collaboration is permitted on the assignments, exam, and other forms of individual evaluation. Cheating, plagiarism, and any form of dishonesty will be handled with the maximum severity permitted under EPFL rules. If you are in doubt whether an action on your part is acceptable, please ask the course staff privately via the staff e-mail list before proceeding. Asking afterward is too late.

## Archived Materials

You can find related materials from previous years below.
Note that the topics covered in the course change from year to year, so archived material might no longer be relevant.

- [How to give a tech talk](talks.md)
- [Final exams](exams/final/README.md)
- [Midterm exams](exams/midterm/README.md)

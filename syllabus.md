---
layout: page
title: Syllabus
catalog: NRES 898
credits: 1
semester: Spring 2017
professor: Dr. Drew Tyre
office: Hardin Hall 416
email: atyre2@unl.edu
phone: 402-472-4054
schedule: ['Tuesdays, 2-5, Online']
office_hours: by appointment
TA: Shivani Jadeja
TA_email: shivanivj@huskers.unl.edu
---

## {{ site.title }} 

{{ page.catalog }}, {{ page.credits }} Credits, {{ page.semester }}

### Professor

{{ page.professor }}

Office: {{ page.office }}

Email (best way to contact me):
[{{ page.email }}](mailto:{{ page.email }})

Phone: {{ page.phone }}


### Times & Location

**Note: class is in different locations depending on the day of the week**

{% for class in page.schedule %}
  {{ class }}
{% endfor %}


### Office Hours

Times: {{ page.office_hours }}

Location: {{ page.office }}

*Note: my schedule gets very busy during the semester so please try to schedule
appointments as far in advance as possible. In general it will be very difficult
to set up appointments less than 24 hours in advance.*


### Course TA

{{ page.TA }}

Email: {{ page.TA_email }}


### Website

The syllabus and other relevant class information and resources will be posted
at [{{ site.url}}]({{ site.baseurl }}/).
Changes to the schedule will be posted to this site so please try to check it
periodically for updates.


### Course Communications

Email: [{{ page.email }}](mailto:{{ page.email }})


### Required Texts

There is no required text book for this class.


### Course Description
 
Computers are increasingly essential to the study of all aspects of
biology. Data management skills are needed for entering data without errors,
storing it in a usable way, and extracting key aspects of the data for
analysis. Basic programming is required for everything from accessing and
managing data, to statistical analysis, to modeling. This course will provide an
introduction to data management, manipulation, and analysis, with an emphasis on
biological problems. Class will typically consist of short introductions or
question & answer sessions, followed by hands on computing exercises. The course
will be taught using R, but the concepts learned will easily apply to
all programming languages.


### Prerequisite Knowledge and Skills

Knowledge of basic biology.


### Purpose of Course

In this course you will learn all of the fundamental aspects of computer
programming that are necessary for conducting biological research. By the end of
the course you will be able to use these tools to import data into R, perform
analysis on that data, and export the results to graphs, text files, and
databases. By learning how to get the computer to do your work for you, you will
be able to do more science faster.


### Course Goals and Objectives

Students completing this course will be able to:

* Create well structured data
* Write simple computer programs in R
* Automate data analysis
* Apply these tools to address biological questions
* Apply general data management and analysis concepts to other programming
  languages and database management systems


### Teaching Philosophy

This class is taught in an online approach, because
learning to program and work with data requires actively working on
computers. Online classes work well for all kinds of content, but I think they
work particularly well for computer oriented classes. 


### Instructional Methods

Students interact in this course both synchronously and asynchronously. Students are provided with either reading or video
material that they are expected to view/read prior to synchronous online sessions. Synchronous sessions will
involve brief refreshers on new concepts followed by working on exercises in
class that cover that concept. While students are working on exercises the
instructor and TA will actively engage with students to help them understand material
they find confusing, explain misunderstandings and help identify mistakes that
are preventing students from completing the exercises, and discuss novel
applications and alternative approaches to the data analysis challenges students
are attempting to solve. For more challenging topics sessions may start with 20-30
minute demonstrations on the concepts followed by time to work on exercises.


## Course Policies


### Attendance Policy

Attendance will not be taken or factor into the grades for this class. However,
experience suggests that students who regularly miss class struggle to learn the
material.


### Quiz/Exam Policy

There are no quizzes or exams in this course.


### Make-up policy

Late assignments will be docked 10% up to one week late, and 20% up to the end of the class, except in cases of genuine emergencies that can be documented by the student or in cases where this has been discussed and approved in advance. This
policy is based on the idea that in order to learn how to use computers well,
students should be working with them at multiple times each week. Time has been
allotted in class for working on assignments and students are expected to work
on them outside of class. It is intended that you should have finished as much
of the assignment as you can based on what we have covered in class by the
following class period. Therefore, even if something unexpected happens at the
last minute you should already be close to done with the assignment. This policy
also allows rapid feedback to be provided to students by returning assignments
quickly.


### Assignment policy

Assignments are due Monday night by 11:59 pm Eastern Time. Assignments should be
submitted via Canvas.


### Course Technology

Students are required to provide their own laptops and to install free and open
source software on those laptops (see [Setup]({{ site.baseurl }}/computer-setup)
for installation instructions). Support will be provided by the instructor in
the installation of required software. Interaction in online sessions is greatly 
facilitated by using a USB connected headset with a microphone. It does not need to be
expensive. The built-in microphone and speakers on a laptop are **not** sufficient.

## UNL Policies

### Students with Disabilities

Students with disabilities are encouraged to contact the instructor for a confidential discussion of their individual needs for academic accommodation. It is the policy of the University of Nebraska-Lincoln to provide flexible and individualized accommodation to students with documented disabilities that may affect their ability to fully participate in course activities or to meet course requirements. To receive accommodation services, students must be registered with the Services for Students with Disabilities (SSD) office, 132 Canfield Administration, 472-3787 voice or TTY.


### Student Code of Conduct

Students are expected to adhere to guidelines concerning academic dishonesty outlined in Article III B.1 of University's [Student Code of Conduct](http://stuafs.unl.edu/dos/code). A first offense will result in a 10% penalty on the assignment. A second offense will result in a grade of zero for the assignment. A third offense will result in a grade of F for the course. Students are encouraged to contact the instructor for clarification of these guidelines if they have questions or concerns. The SNR policy on Academic Dishonesty and procedures for appeals are available [here](http://snr.unl.edu/employeeinfo/information/employeehandbook-single.asp?infocode=S162).


### Netiquette and Communication Courtesy

All members of the class are expected to follow rules of common
courtesy in all email messages, threaded discussions and chats.


## Getting Help

For issues with technical difficulties for E-learning in Canvas, please contact the UF Help Desk at:

* Learning-support@ufl.edu 
* (352) 392-HELP - select option 2
* https://lss.at.ufl.edu/help.shtml 

Any requests for make-ups due to technical issues MUST be accompanied by the
ticket number received from LSS when the problem was reported to them. The
ticket number will document the time and date of the problem. You MUST e-mail
your instructor within 24 hours of the technical difficulty if you wish to
request a make-up.

Other resources are available at http://www.distance.ufl.edu/getting-help for:

* Counseling and Wellness resources
* Disability resources
* Resources for handling student concerns and complaints
* Library Help Desk support

Should you have any complaints with your experience in this course please visit
http://www.distance.ufl.edu/student-complaints to submit a complaint.

Most importantly, if you are struggling for any reason please come talk to me
and I will do my best to help.


## Grading Policies

There will be 11 equally weighted assignments. One problem from each assignment
(selected at the instructors discretion after the assignments have been
submitted) will receive a thorough code review and a detailed grade. Other
problems will be graded as follows:

* Produces the correct answer using the requested approach: 100%
* Generally uses the right approach, but a minor mistake results in an incorrect
    answer: 90%
* Attempts to solve the problem and makes some progress using the core concept:
    50%
* Answer demonstrates a lack of understanding of the core concept: 0%

### Grading scale

- **A 90-100**
- **B+ 87-89**
- **B 80-86**
- **C+ 77-79**
- **C 70-76**
- **D+ 67-69**
- **D 60-66**
- **F <60**


## Course Schedule

The details course schedule is available on the course website at:
[{{ site.url }}/schedule]({{ site.baseurl }}/schedule).


**Disclaimer:** This syllabus represents my current plans and objectives. As we
go through the semester, those plans may need to change to enhance the class
learning opportunity. Such changes, communicated clearly, are not unusual and
should be expected.

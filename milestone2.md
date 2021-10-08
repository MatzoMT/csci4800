# Milestone 2: Definition and Related Work
[Back to Home](https://matzomt.github.io/csci4800/)

## A. Task/Problem Definition
### Introduce Your Problem
**Problem**: The Grades section on eLC does not clearly reflect a student’s standing in the course, since for many classes the current “total” grade is not displayed, nor are assignment categories and weights. This makes determining a student’s current grade in the course difficult.
 
While customizability for instructors is welcome, it also leads to large inconsistencies in how the Grades page is displayed to students from class to class. There is a lot of variability in how much work the student must perform in order to determine their true grade, causing confusion for students. This is a large contributing factor to the lack of clarity students face when trying to determine their overall position in any given course.
 
While eLC has all the properties needed of a well-structured gradebook and fits the appropriate conceptual model, we find the system has subpar discoverability and visibility on the instructor end, due to the lack of signifiers for how to implement certain functions into the gradebook. There are many menus to navigate through in the UI, partially because of all of the customizability options, which can make for a cluttered and confusing experience for the instructor. Despite the functionality being available, these functions are not made immediately clear as affordances of the system. While it is evident that the system affords entering grades for each student, for example, it is not clear that instructors can categorize assignments because the option is hidden behind several clicks. Instructors may have to spend some time digging around in menus or documentation to figure out how to set up a gradebook to their liking -- UGA also provides instructors a lengthy guide to navigating Grades on eLC. [18] While the main problem we identified is the lack of consistency in the Grades page for students, a closer examination reveals that the problem is largely caused by the instructor-side design.
 
**Theme**: This problem surrounding the Grades section of eLC connects with the theme of face-to-face instruction, even though it is not entirely unique to face-to-face learning. There are unique factors at the intersection of an online gradebook and face to face learning which may exacerbate the confusion. For instance, students may physically turn in assignments or are handed grades on paper that are yet to be reflected in the online gradebook, causing uncertainty about the accuracy of grades reported in eLC. Additionally, a student’s grades can be an indicator of a student’s commitment to attending classes in person. In-person attendance for a student has a strong correlation with test scores, and this correlation holds true for differences in institution and subject and attendance policies [1]. 
 
**Interactions**: We have listed out a typical workflow for both students and instructors below, using the *Seven Stages of Action* structure. 
 
Anecdotally, as students ourselves, we are familiar with the flow of checking our grades on eLC, and mapped out a typical interaction. While we were not initially as familiar with the instructor’s stages of action, we were able to gain access to a sample eLC course to examine how the Grades page and grading process looked from the instructor’s viewpoint. With this as an example, we were able to recreate a typical use case for entering grades from a paper assignment into eLC. We also researched to ascertain whether our experiences with eLC were, in fact, typical.

The University of Colorado Boulder published a Learning Management System Evaluation Report for their students in 2016 and their faculty in 2017 -- this school primarily uses the Brightspace Desire2Learn (D2L) Learning Environment platform, which is what eLC at UGA is based on. In the survey of students’ experiences with learning management systems, some of the key findings were that “Students wish that faculty would use the D2L gradebook more effectively” and “Students are frustrated with faculty’s inconsistent configuration of D2L courses.” [5, pg. 1]. Specifically, the study indicated that students at UC Boulder had the most comments and complaints about the following pain points: ”Gradebooks not kept up to date,” “Gradebooks not set up to calculate final grade,” and “Gradebooks not set up to display current course grade” [5, pg. 8]. 
 
In the UC Boulder survey of teachers' experiences with the various learning management platforms, it was found that over 90% of UC’s faculty used D2L, and one of the most commonly used functions was the Gradebook. Despite it being one of the more frequently used features, only “64% of survey participants indicated that they were satisfied with the Gradebook/Grades Tools, and a large proportion indicated that they are dissatisfied” [6, pg. 7]. A majority complained that the gradebook was hard to use, lacked adequate features, and was not well integrated with other features of the platform [6, pg. 9]. 
 
We also did our own research to find and evaluate online student and professor sentiment for the D2l/Brightspace gradebook and compiled the results in a spreadsheet [15]. We classified each post as either having a positive (3), neutral (2), or negative (1) sentiment towards the D2L Grades system. The most common score, mode, was 1 and the mean was 1.3, indicating a broadly negative sentiment. The metrics indicate that the student sentiment is overall one of negative feelings and confusion towards the Grades page.
 
Our research indicates that the issues we identified are indeed problems not only for ourselves, but other users of D2L as well. Thus, we are confident that the interactions outlined below are typical.
 
Seven Stages of Action, for Students:
1. **Goal**: The student wants to view their grades in a course.
2. **Plan**: The student considers the means by which they will access the grades section for that course, such as via mobile or by computer.
3. **Specify**: The student picks one of the means described above. 
4. **Perform**: The student navigates to the grades section for that course on eLC and views the grades for that course.
5. **Perceive**: Depending on the course, the student may not understand their grade at first due to inconsistent grading structures or the differing layouts of the grades page. The student may be able to view the current “final” grade for the course, only if available.
6. **Interpret**: If a current “final” grade is not available, the student may have to manually perform calculations using another website or a calculator in order to determine their current standing in the course. If the grades are not easy for the user to understand, or if the current number of grades indicates the student is underperforming, the student may believe that they are in a position where they can no longer do anything to improve their grade.
7. **Compare**: The student may reflect on the experience in relation to other experiences with different gradebooks and be less sure the task was completed and evaluated successfully. If the student needed to use external resources (such as cross-referencing the syllabus to determine assignment weight or using a grade calculator tool) to accomplish the task of determining their current grade in a course, the student may not be satisfied with the eLC page as it alone was not enough to accomplish their goal.
 
Seven Stages of Action, for Instructors:
1. **Goal**: The instructor wants to enter the grades for each student for an in class assessment.
2. **Plan**: The instructor must consider which assignment they wish to enter grades for and whether it is an assignment already on eLC or one that was paper graded. Because it is the latter, they must also have the graded papers or exams ready in front of them.
3. **Specify**: The instructor considers their action sequence - with the grades on paper in front of them, they then plan to first enter the assignment into the eLC gradebook, and then enter in the grades.
4. **Perform**: The instructor navigates to the “Grades” tab on eLC, and then to the “Manage Grades” menu tab. From there, they must create the assignment and choose the appropriate settings - for example, whether it is a numeric or letter grade to be displayed. Then, the instructor will navigate to the “Enter Grades” menu tab. They manually enter the grades for each student by referencing the graded assignment page and entering it into the created assignment’s column in the corresponding row for each student’s name.
5. **Perceive**: Once the instructor has entered the grades, the “Enter Grades” tab shows all of the grades under that assessment’s column as filled in.
6. **Interpret**: Depending on how the instructor has their gradebook setup the grades for a given assignment may show in a different category than intended or only in certain areas of the course. This may make it hard for the instructor to judge which students are struggling and/or need more help understanding certain coursework. 
7. **Compare**: The instructor may reflect on the experience of entering grades into the gradebook and compare it to experiences with different learning platforms and be less satisfied due to the lack of discoverability in comparison to other platforms. The instructor has completed the goal, but it may have been more complex than expected if they wanted to, for example, set a category for that assignment.

### Identify your potential users
There are two main user populations affected by this problem with eLC: Students and Instructors (including professors, TAs, etc.) at the University of Georgia. As eLC is based on the Brightspace (Desire2Learn) Learning Environment, students and professors at other universities which use Brightspace as a base for their school-wide learning management system likely face similar problems, yet our problem is focused on eLC specifically. The gradebook in eLC differs based on a student view and an instructor view.

As students must contend with presentation inconsistencies across all courses in order to determine their overall standing, they become the most impacted stakeholder in this issue. Grades have been linked to students’ feelings of autonomy, where the grades a student makes in a class can influence their future class scheduling and career planning decisions [2]. If the eLC gradebook were to more clearly reflect a student’s standing in the course, it may alleviate anxiety and save students’ time manually calculating their grades.

Professors are also impacted as a stakeholder. For instance, depending on their chosen presentation of the eLC gradebook, they may have to manually calculate students’ final grades, creating otherwise unnecessary work for them at the end of each semester. By better designing the system to make it easier for professors to find calculated final grades, they would be able to save time. Instructors (not just professors, but also TAs) may also be affected negatively if students bombard them with questions about their present academic standing, or when students become reluctant to dedicate more time or attendance in improving their grade in the class. A solution to the student-side of the issue would positively impact professors as well. Professors perform related tasks such as calculating students’ final grades (if their gradebook is not set up so that it is automatic) and transferring final grades over from eLC to Athena.

## B. Analysis of Existing Solutions
### Describe Existing Solutions
Brightspace/D2L offers well documented information of adjusting the gradebook and eLC has tools to allow professors to configure the gradebook. There is a lot of flexibility provided. An issue, however, is that it is largely text based and there is a lot of manual set up that professors must do if they want their gradebook set up to match the grading structure outlined in the syllabus. UGA provides lengthy documentation for the gradebook functionality on eLC, but the length may actually discourage a thorough reading. [18] Because of this, it is often easier for professors to just input the grades with minimal extra configuration and manually calculate the final grades at the end. The Brightspace provided documentation for gradebook setup is also provided as a source. [3] As mentioned above in section A, University of Colorado Boulder surveys of both students and professors reveal that there are several pain points regarding the existing eLC gradebook. Students find the inconsistencies frustrating, and instructors find the gradebook system difficult to use [5][6]. Overall, it has been reported that Brightspace has a very steep learning curve compared to other learning management systems. [17]

Other educational technologies have existing implementations of an online gradebook as well. We examined Canvas [4] and Blackboard [5] specifically to see if they had additional features that eLC lacks, or if there are differences in how the same features are displayed.

Canvas has many of the same basic features as D2L. Canvas’s instructor view clearly shows an instructor how many assignments a student is missing or has submitted late. This feature can prompt an instructor to individually notify a student about missing work, as well as provide an extra credit option depending on what percent of students submitted an assignment late. Canvas will also give an easily accessible rating of how well the student is participating in the class and how often they navigate to the page. [11]

Canvas has some features of grade organization that eLC either lacks or makes difficult to access. For instance, Canvas highlights “Assignment Groups” which are equivalent to eLC categories, and gives the gradebook structure (helpful for students when interpreting their grades). Having the “add group” option as a separate button from “add assignment” helps to highlight this feature in the UI -- in eLC, by contrast, the category feature is hidden behind the same button used to add new assignments. Additionally, Canvas allows instructors to rearrange graded items in the gradebook by dragging and dropping them to a new location - this is a useful feature for instructors to be able to logically organize the assignments and help students make more sense of the grade organization, which eLC lacks. [11]

The student view of Canvas also has the ability to tell the student which assignment they are missing or submitted late, including the original score the user would have scored and the late penalty. This useful feature reduces the need for the instructor to specifically comment on the student’s grade breakdown. [12]

Canvas provides many third-party app integration with its services, such as connection to social media, and it is also available in a free open-source version. These features likely helped Canvas unseat the former learning management system leader, Blackboard, as the leading system in U.S. higher education institutions. [16] However, an organization must pay for the hosted service in order to access additional paid features. [17]

Blackboard’s instructor view provides an easy-to-interpret and intuitive UI with additional features not offered by eLC. The platform clearly shows each student’s letter grade in the course as well as any assignment submitted by the student that has not been graded. It directly prompts the instructor to grade these assignments in the “global grades page” home view. This feature can encourage instructors to grade assignments more quickly due to its simple interface that makes good use of discoverability and signifiers. [13]

Blackboard also provides an easy way for instructors to rearrange graded items by dragging and dropping them to a new location - this is a useful feature for instructors to be able to logically organize the assignments and help students make more sense of the gradebook, similar to Canvas but unlike eLC. Instructors can configure their gradebook to their liking by accessing the “Gradebook settings” page. Similar to eLC, it appears as though the settings to add categories must be accessed through this menu. [13]

Blackboard’s student view for the grades section condenses separate features given by eLC into a single pane. The grades section not only shows the due date for each assignment listed, but also shows whether the assignment has been submitted, graded, or reviewed. There is also an Overall Grades section that provides the total grade for the course and a breakdown of assignments and their current grades based on the assignment’s weight and influence in the grade total. [14]

Overall, the UI of both the gradebook settings page for instructors and the Grades view for students on Blackboard is more pleasing and attractive due to the use of colors as letter grade indicators (green for A, yellow for C, etc.) and icons to indicate the category of an assignment. [13][14] However, despite Blackboard’s more intuitive UI compared to Canvas and D2L, its learning curve has been reported to be steeper than the average gradebook technology. [17]

There are also separate Student Information Systems that some school systems and universities use to record grades, instead of learning management systems with this functionality built in. These student information systems seem to capture much of the same information that is found on Athena at UGA, but with the gradebook functionality added. Capterra, a software reviews company, published a survey on Learning Management Systems conducted in July 2020, and found that both LMS and SIS implement gradebook functionality, which can cause issues in schools that use both [7]. 

### Describe potential guidelines and solutions
**Guidelines** - Fortunately, it seems as though the above solutions are built with universal usability in mind, and since they are used across many types of schools and institutions, including public institutions. This means each software overall conforms to WCAG accessibility guidelines, including the Gradebook views. [8][9][10] In addition, the basic guidelines for designing user interface software, as laid out by Smith and Mosier, have been followed. [19] For instance, data entry for instructors is supported with mouse and keyboard input, data visualization is laid out clearly in tabular formats, and there is generally a clear sequence of actions for both students and professors. 

**Principles** - Potential solutions should ideally conform to Norman’s Principles of Good Design and other such sets of principles. [20] All three systems do a good job of providing a match between the online system and the real world. Each online Grades system roughly matches the spreadsheet format that would be found in a pen-and-paper version of a gradebook. This makes the conceptual model easy to understand, as the user already knows what to expect from the interface due to having dealt with a physical analogue. In addition, each platform has generally aimed for consistency, by ensuring that any icons or colors consistently have the same meaning across the UI. Also, for the instructor view of the gradebooks, each system has done a good job of keeping the user, the instructor, in control, by providing lots of options to configure and tweak the structure of the grades and assignment settings. Furthermore, Canvas’s and Blackboard’s features on the instructor end show an appeal to discoverability because much of their configuration tools are made available in the grades section without having to navigate to hidden menus or other pages to access those key features. The same cannot entirely be said of eLC/D2L, which tends to hide options and functions behind a few clicks, and does not clearly signify where they are located. It would certainly best serve our users to ensure visibility of gradebook functions identified as important by students, so that instructors have an easier time finding these settings and can implement them more frequently.

## C. Proposed Solution
### Propose your solution
Upon examining the current implementation on eLC and the features available on Brightspace, we realized that many of the features desired by students are available. The issue lies in the implementation on the instructor end - because there are so many choices for customization, the overall experience becomes difficult to navigate for instructors, while also leading to an inconsistent format in the student view. There is a lot of choice in how instructors can choose to set up their gradebook, and it can be difficult to navigate through all the menus. This difficulty means that many settings that are important to students are left ignored.

To alleviate these issues for both students and instructors, we propose the following:

We believe it may better serve our students to have some highly desired options be set as the default, such as final calculated grades being automatically shown and updated. It is likely that many professors would not object to having these options be default, but they simply do not go through the effort to enable them. Currently, eLC Gradebook affords these options, but the professor must choose to enable it. If these settings had the property of being opt-out instead of opt-in, it would likely lead to increased usage of those settings and thereby increase the utility of the average Grades page for students. This would give students a more consistent and more informative view of the Grades page. In addition, these settings could also be highlighted in UGA’s help manual for professors setting up their gradebook -- while this is not a design change to the eLC UI itself, noting the students’ preferences as recommended in the documentation further encourage instructors to enable those options. [18]

Adding categories in the gradebook is currently rather cumbersome and a little confusing, as the option to add a category is part of the “New” dropdown under the section “Manage Grades,” and thus is a little hidden. This is unfortunate, because adding categories is a useful feature that helps to match up the gradebook with the syllabus structure which is a useful indicator to students. Potentially, the “Manage Grades” tab could be renamed to a more appropriate signifier such as “Manage Gradebook” to better indicate to instructors that this page includes functions for setting up the structure of the gradebook and assignments. Additionally, we believe it would better serve the instructors to get rid of the “New” dropdown on that page and instead split it out into two separate buttons: “New Category” and “New Item” to make the options more visible and clear. Finally, changing the category of an item without having to click through another page could be accomplished by adding “drag and drop” functionality to grade item rows, making categorization of assignments much easier and more intuitive.

Signifiers that indicate to professors when their choices are not displaying vital information to students may also be helpful - for example, when entering a numeric grade without any indication of how many total points were possible, a red warning message could display on the screen before the instructor can save the assignment. This would let a professor know they may have forgotten to include the total points available. Reminders such as this could make gradebook setup a bit easier for professors, by reducing the mental memory load required when filling out the form, and make viewing grades a more consistent experience for students, by ensuring each numeric grade has a corresponding “total points” provided.

### How will you measure success?
A survey of users, including both students and professors, who indicate their satisfaction with the updated design. Satisfaction may be measured on several metrics such as ease of use (for professors inputting grades or setting up a gradebook) or ease of interpretation (for students when viewing the grades). 

Another way to measure the success of the design is to have teachers report the amount of time it takes to perform certain standard tasks, such as updating grades, adding a new category, updating categories for graded items, and changing the gradebook configuration, to see if this time has changed from the amount of time it took for the teachers using the original design. This can allow us to see if this new design is quicker and doesn’t cause teachers to waste more time than before.

A design could be deemed as successful when someone who has never used the design can easily navigate it. This can be a criteria because 2 out of 4 of our group members have never used the original design of the instructor view for eLC. These 2 students can now try to create a gradebook using the new design, and this will allow us to determine if, as a new user, the instructor-side design is not intimidating and easy to navigate.

On the student end, a successful design may also be judged by the overall end grades of the students to see if this updated design allows more transparency for students, which in return creates a more motivated desire to get the grades needed to excel in the class. This causation may be hard to determine and is just a hypothesis, however, so a more straightforward approach would be to survey students to determine whether the new eLC gradebook is showing them the information they were looking for.

## D. Summary Video
Link to video: <https://youtu.be/XVW4yPxPOwY>

{% include_relative youtubeMilestone2.html %}

## Sources
[1] LeBlanc, <http://communication.utsa.edu/leblanc/articles/art31.pdf>

[2] Chamberlain, <https://journals.sagepub.com/doi/full/10.1177/1469787418819728>

[3] eLC documentation <https://documentation.brightspace.com/EN/le/grades/instructor/set_up_grade_book.html>

[4] Canvas documentation <https://community.canvaslms.com/t5/Instructor-Guide/How-do-I-use-the-Gradebook/ta-p/701>

[5] UC Boulder Student Study
<https://www.colorado.edu/lms/sites/default/files/attached-files/lms_eval-stud_1.pdf>

[6] UC Boulder instructor study <https://www.colorado.edu/lms/sites/default/files/attached-files/lms_eval-fac_0.pdf>

[7] Capterra LMS survey <https://www.capterra.com/learning-management-system-software/user-research>

[8] Canvas accessibility <https://www.instructure.com/canvas/accessibility?newhome=canvas>

[9] D2L accessibility <https://www.d2l.com/accessibility/standards/>

[10] Blackboard accessibility <https://www.blackboard.com/blackboard-accessibility-commitment>

[11] Canvas instructor view <https://www.csustan.edu/office-academic-technology/canvas/canvas-how-gradebook-setup-and-grading>

[12] Canvas student view <https://community.canvaslms.com/t5/Student-Guide/How-do-I-view-my-grades-in-a-current-course/ta-p/493>

[13] Blackboard Instructor features, pros and cons
<https://help.blackboard.com/Learn/Instructor/Ultra/Grade/Navigate_Grading>

[14] Blackboard Grades Student View
<https://help.blackboard.com/Learn/Student/Ultra/Grades>

[15] Spreadsheet analyzing student sentiment of eLC Gradebook
<https://docs.google.com/spreadsheets/d/1k4ryR_frWc1d-duoLC8xsZjQlYNBuNmeGjvWkQCUQ2U/edit?usp=sharing>

[16] Existing solutions market share
<https://www.insidehighered.com/digital-learning/article/2018/07/10/canvas-catches-and-maybe-passes-blackboard-top-learning>

[17] Pro-cons of Blackboard, Canvas, D2L
<https://elearningindustry.com/learning-management-systems-for-higher-education-overview-popular>

[18] UGA Guidelines on eLC Gradebook Setup
<https://help.elc.uga.edu/assessments/gradebook/grades_setup/>

[19] Smith and Mosier, Guidelines for Designing User Interface Software <http://www.hcibib.org/sam/4.html>

[20] Norman's Principles of Good Design <https://michaelcotterell.com/hci/2021fa/html/ddq/2021-09-21-TUE.html#term-Norman-s-Principles-of-Good-Design>
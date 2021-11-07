# Milestone 3: Design Alternatives
[Back to Home](https://matzomt.github.io/csci4800/)


## A. User Experience Requirements
### Activities
We have grouped our user stories by activities available. With each group, we italicized the stories chosen which we believe are most relevant, and provided a brief justification as to why the others were not chosen. Additionally, we provide a more detailed breakdown with justification and evidence provided for each chosen user story.

**Activity: viewing grades**
1. As a student user, I want to view my graded assignments for a class, so that I can know my performance on specific assignments.
2. As a student using the eLC gradebook, I want to be able to understand at a glance how much I got on an assignment and how much it is weighted in the category.
3. As a student using the eLC gradebook, I want to view the total points available on a numeric assignment as well as the points I earned, so that I can know what percentage I scored.
4. As a student using the eLC gradebook, I want to be able to understand my grades clearly so that I know which sections of the class I should focus more on.
5. As a student using the eLC gradebook, I want to be able to calculate my current grade so that I know the grades I need to earn in order to obtain a certain letter grade.
6. *As a student user, I want to view my overall calculated grade in a course so that I can understand my overall performance in the class.*

Justification: While all of these user requirements for students are important, user story 6 is generally encompassing many of the other stories. Additionally, upon analyzing in Milestone 2, we found that almost all of the features desired by students, as described in stories 2, 3, and 5, are already available in eLC, but the issue lies in inconsistent implementation on the instructor end. Thus, there are not many changes required on the student view of the eLC gradebook, as we believe that a redesign of the instructor-side UI will automatically resolve many of the student requirements.

**Activity: viewing gradebook**
1. As an instructor user, I want to view a specific student’s grade on a specific assignment so that I can double check if I entered it correctly.
2. As an instructor user, I want to view each student’s final grade in my course so that I can enter their final grades into Athena.
3. As an instructor, I want to be able to view differences in grades (e.g. late penalty, quiz time expired, never turned in) which can be more than just a simple number
4. As an instructor using the eLC gradebook, I want to be able to see which students have not submitted an assignment so that I can notify them to complete an assignment.

Justification: While instructors viewing the eLC gradebook is a related activity when considering the eLC grades system as a whole, it is not as relevant to the overall solution, which requires addressing how the gradebook structure looks on the student side. Thus, these user requirements are not relevant to our problem.

**Activity: gradebook setup**
1. As an instructor user, I want to configure my gradebook to match the structure of my course so that I can enter grades that accurately reflect the nature of my assignments and my preferred grading style.
2. As an instructor user, I want to be able to adjust my gradebook configuration so that I can adapt throughout the semester if needed.
3. *As an instructor user, I want some easy sample frameworks available to use so I can choose a functional and user-friendly set-up without having to know every intricacy of eLC.*
4. *As an instructor user, I want to configure a gradebook with features important to students as well as to myself, so that my students are not confused regarding their grade view, I will have to spend less time answering their questions, and I can match my preferred grading style.*

Justification: User stories 3 and 4 were the most central to our goal to make configuration of the eLC gradebook easier for instructors and and more uniform for students. We feel that the other stories they will be less relevant to address for this project, which involves creating a visual representations of the selected user stories, and are not directly related to the proposed solution outlined in Milestone 2. For instance, user story 1 is an important issue for instructors, but is less directly relevant to addressing the specific problem we identified which ultimately deals with how the gradebook looks on the student side. User stories 3 and 4 specifically address making the UI more intuitive for the instructor to configure the gradebook while matching student needs, and addressing these will include designs to make user story 1 easier as well. User story 4 is particularly important as it directly ties together the student and instructor desires.

**Activity: creating assignments and categories**
1. As an instructor using the eLC gradebook, I want to create an assignment from scratch so that I can enter grades for assignments I handed out in person and graded on paper.
2. As an instructor user, I want to create a grade item that was assigned on eLC so that I can take advantage of the eLC assignments/quizzes section, with less work for me.
3. As an instructor using the eLC gradebook, I want to be able to clearly note the total points available when creating a numeric assignment so that I can more easily calculate grade averages for students at the end of a course.
4. *As an instructor using the eLC gradebook, I want all of the important fields emphasized when creating a grade item so that I do not forget anything and the process is smooth.*
5. As an instructor user, I want to add categories to my gradebook so that I can match my syllabus weighting structure.
6. As an instructor using the eLC gradebook, I want to be able to appropriately categorize a grade item so that I can more easily determine a student’s final grade.
7. *As an instructor user, I want to be able to appropriately categorize a grade item so that I can better match my syllabus weighting structure.*

Justification: The first two user stories are not as immediately relevant to our problem, though they are related activities available on the eLC Grades page for instructors, so we did not highlight them as part of our potential solution. User story 3 captures an issue related to our problem, as described in our Proposed Solution section in Milestone 2, but it falls under user story 4, which is a more general version. As such, we chose user story 4. We also chose user story 7 as one of the more relevant stories, also described in our Milestone 2 proposed solution. User story 7 encompasses user story 5 and 6, as they are a common group.

**Activity: entering grades**
1. As an instructor user, I want to have a compatible interface to allow entering grades much easier and less intimidating, so that I can quickly get grades uploaded.
2. As an instructor using the eLC gradebook, I want to be able to view the status of my students’ assignment submissions so that I have a better understanding of which grades I have already inputted or need to be graded.

Justification: As a group, we felt the issues brought up in user stories in this section would be better addressed by stories regarding creating assignments and categories. This is because the actual activity of entering grades is not as immediately relevant to the problem we outlined in Milestone 2 - more issues can be traced back to the gradebook setup and structure rather than the grading process itself - and as such, would not be as valuable to consider for our solution.

### Top User Stories
**As a student user, I want to view my overall calculated grade in a course so that I can understand my overall performance in the class.**
- Justification: The main problem we identified in Milestones 1 and 2, and the potential solution described in Milestone 2, all center around the need for students to understand their overall class performance and the fact that eLC currently often fails to meet that requirement.
- Evidence: The University of Colorado Boulder published a Learning Management System Evaluation Report for their students - this school primarily uses the Brightspace Desire2Learn (D2L) Learning Environment platform, which is what eLC at UGA is based on. The survey indicated that students at UC Boulder had the most comments and complaints about the following pain points: ”Gradebooks not kept up to date,” “Gradebooks not set up to calculate final grade,” and “Gradebooks not set up to display current course grade” [1, pg. 8]. 

**As an instructor user, I want to configure a gradebook with features important to students as well as to myself, so that my students are not confused regarding their grade view, I will have to spend less time answering their questions, and I can match my preferred grading style.**
- Justification: Instructors are also an affected stakeholder to the gradebook issue because there are barriers within D2L that can prevent them from configuring a more intuitive gradebook. However, our proposed solution highlights the fact that if professors can configure the gradebook to match their course structure, it will make grade interpretation easier for students. Existing guides to configuring a D2L/eLC gradebook, namely the UGA guide and D2L’s guide, are very text-heavy and expose the flaws of eLC’s UI compared to other learning management systems. eLC also fails in several principles of good design, such as many hidden and nested functionality and a lack of good signifiers.
- Evidence: In Brightspace’s guide to configuring a D2L gradebook, there are no visuals provided to instructors [6]. This issue makes it more difficult for instructors who are not accustomed to D2L to learn how to configure the gradebook to meet their needs, especially considering that the eLC/D2L UI is lacking. The UI for configuring the eLC gradebook is not intuitive in comparison to other gradebook technologies such as Canvas and Blackboard; UGA’s eLC guide for faculty reveals that eLC’s grade setup process is also very text heavy without assistance via diagrams and colors [5].

**As an instructor user, I want some easy sample frameworks available to use so I can choose a functional and user-friendly set-up without having to know every intricacy of eLC.**
- Justification: A major part of our problem analysis was the inconsistency in student views of the Grades page, stemming from the vast options for customization available to professors. However, many options that students desire take some time to set up. Having some sample frameworks to choose from as starting points may make the Gradebook schema set up process easier for professors who are not as comfortable with technology and/or do not want to spend a lot of time setting up a gradebook. In contrast, the gradebook configuration pages for both Canvas and Blackboard possess a more user-friendly interface with better signifiers and discoverability in the form of distinct colors and icons that eLC lacks.
- Evidence: In the University of Colorado Boulder study focusing on faculty experiences with the Desire2Learn platform, many instructors noted the gradebook was both hard to use and lacking adequate features [2]. Many students at UC Boulder also noted frustration with the basic configurations used by instructors [1]. We believe that adding sample frameworks may ease this process for instructors and allow for options that better accommodate student desires as well. Canvas instructor view documentation [7], Blackboard Instructor features [8], reveal features that eLC lacks.

**As an instructor user, I want to be able to appropriately categorize a grade item so that I can match my syllabus weighting structure.**
- Justification: Categorization of gradebook items is relevant to our problem’s proposed solution because making it easier for professors to have appropriate and easier categorization of grade items would lead to more structured gradebooks across the board, making it easier for students to interpret the Grades page. Currently, categorization in D2L is lacking and is hidden behind many menus/clicks and means this user requirement is not adequately fulfilled.
- Evidence: When our group members analyzed online sentiment of D2L via Reddit comments, we saw comments from many instructors using the platform. For instance, one professor noted that “Setting up grades and assignments are very confusing” and another agreed, replying “Currently using D2L and trying to figure out why important features are buried in weird places” [4]. The categorization of grade items is one such example, where one must go through several clicks just to create a new category or change the category of an existing assignment. In Milestone 2, we found that alternate LMS platforms such as Canvas and Blackboard both had easier drag-and-drop interfaces to move grade items to categories, so we believe that D2L/eLC would benefit from having similar functionality as the industry leaders, and it would make the platform easier to use, addressing common complaints [7][8].

**As an instructor using the eLC gradebook, I want all of the important fields emphasized when creating a grade item so that I do not forget anything and the process is smooth.**
- Justification: The main problem of students having an inconsistent gradebook view stems from the vast availability of options available to instructors when creating and entering gradebook assignments. Often, though, this means the menu on the instructor side is cluttered up and instructors may forget certain important fields when creating the assignment. Adding some signifiers that these fields are often important to student users, such as highlighting and warning prompts, would help professors remember which fields are important to include.
- Evidence: One of Shneiderman et al.’s Eight Golden Rules for Interface Design is to *Reduce short term memory* [3]. This is often classed as an important design feature because it makes an interface easier and more convenient to use for the user, and involves making options and information available upfront [3]. In this case, adding important signifiers would mean that professors would have less to remember when creating a grade item, making the interface easier to use and ultimately making the gradebook page more useful for students. This also would contribute to making the overall interface of the D2L Grades system easier to use, which was a common complaint found in UC Boulder’s faculty survey of LMS [2].

## B. Ideation and Preliminary Designs
### Ideation
**User Story 1**: As a student user, I want to view my overall calculated grade in a course so that I can understand my overall performance in the class.

Ideation Screenshot:
![jamboard-1](assets/images/jamboard-1.PNG)

Top Ideas:
- Have the overall calculated grade set up to be displayed and updated by default in its own section. 
- Employ a grade calculator built into the eLC grades page to calculate overall grade (both current and potential). 


**User Story 2**: As an instructor user, I want to configure a gradebook with features important to students as well as to myself, so that my students are not confused regarding their grade view, I will have to spend less time answering their questions, and I can match my preferred grading style.

Ideation Screenshot:
![jamboard-2](assets/images/jamboard-2.PNG)

Top Ideas:
- Have certain fields be opt-in instead of opt-out by default, for instance, displaying and updating final grade. 
- Add visuals and colors beyond just a plain text form for the gradebook setup wizard to make the UI clearer and more intuitive.  


**User Story 3**:  As an instructor user, I want some easy sample frameworks available to use so I can choose a functional and user-friendly set-up without having to know every intricacy of eLC.

Ideation Screenshot:
![jamboard-3](assets/images/jamboard-3.PNG)

Top Ideas:
- Have a visual display of cards with sample frameworks to select, which are customizable after selection. 
- Provide clear explanations for which framework or options are best for which use-case, including explanations for student-friendly settings.  


**User Story 4**:  As an instructor user, I want to be able to appropriately categorize a grade item so that I can match my syllabus weighting structure.

Ideation Screenshot:
![jamboard-4](assets/images/jamboard-4.PNG)

Top Ideas:
- Provide a form or table page to add categories in bulk/at once, instead of needing to click through the whole menu page for each one.  
- Provide a drag and drop interface to categorize grade items or order the categories. 


**User Story 5**: As an instructor using the eLC gradebook, I want all of the important fields emphasized when creating a grade item so that I do not forget anything and the process is smooth.

Ideation Screenshot:
![jamboard-5](assets/images/jamboard-5.PNG)

Top Ideas:
- Update the UI of the grade item creation page with clearly defined sections (weight, effect on grade, etc.) separated by color or font weight. 
- Display warning messages if certain student-friendly features are missing such as total points are not entered in a numeric assignment, or if item hasn't been categorized.

### Wireframes

Source Figma File:

User Story 1
{% include_relative assets/html/figma/wireframe1.html %}
Justification:
We chose to display the final calculated grade for the course at the top of the page because we felt that this location would be the most realistic and attention-grabbing for a student wanting to view their final grade. Furthermore, courses that do include the final grade on eLC are already included at the top of the page, which seems intuitive as one can expect that students would want to view their total grade first before looking at the makeup of their grade. Therefore, we decided to stay in line with eLC’s existing functionality. The main change in our design is that this score would be displayed by default, a commonly requested feature by students using LMSs [1].

We chose to build out a grade calculator functionality on the side of the current grades table. We chose the right side because it is immediately visible to the student, compared to a calculator on the bottom, which may be missed if the grades table is long and the user must scroll down. We chose the right hand side because research has shown that most users tend to trust information more and can operate tasks easier on the right hand side of the screen, especially since the majority of users are right handed [11]. We also modeled the “Category Breakdown” table and general structure of the calculator to be similar to Canvas’s grade calculator, which is a market-leading LMS with grade predictor functionality built-in [9] [10]. We believe the demonstrated popularity of Canvas and its gradebook functions would make it a good model for eLC.

User Story 2
{% include_relative assets/html/figma/wireframe2.html %}
Justification:
We chose to make the setup wizard automatically have the Final Grade Release option checked by default, and make it an opt-out setting, so that instructors are more likely to keep this option. [12] This tendency for an agent to accept the default condition is sometimes called the “Default Effect” [13]. We anticipate that this will lead to more students being able to view their final grades in a course and a more consistent and informative experience for students. We also have an exclamation point in red to show that it is an important setting. We mirrored this same pattern for keeping the final grade automatically updated. This is defaulted and shows an exclamation point to emphasize the importance. 

On these pages, we followed eLC’s existing pattern of using checkboxes and radio buttons for certain options, as eLC’s current solution already follows best practices for checkboxes and radio buttons. [14]

We thought it would be helpful to have a completion bar at the top which shows how far along in the grading process an instructor is so it’s less unknown and more encouraging to get through. We also incorporated the use of color and better sizing / font weights for our page because we feel this will make the page more visually appealing than a long plain text form and less intimidating for instructors, especially those new to setting up a gradebook in eLC.

User Story 3
{% include_relative assets/html/figma/wireframe3.html %}
Justification:
In this story's wireframe, we did not separate them out into two different series of frames because we felt that both proposed ideas dealt with different aspects of the same user story.

We chose to design the frameworks as separated tiles in order to make the format easier to read versus a chart or a plain text layout. By using tiles, instructors will clearly be able to see the grading structure and schema of each of their classes side-by-side to facilitate easier modification and comparison. This same structure was also carried over to adding frameworks, where tiles would make it easier to compare different frameworks. For selecting or adding a framework, we decided to use a green button to differentiate between the different options, as well as to add more color coded options to eLC, which lacks the feature of using color as a signifier when compared to other LMS mediums such as Blackboard. [8]

As a result of better use of colors and a more visual layout with the tiled framework options, we believe that the users will be more engaged with the UI compared to the current version, which is a plain page in tabular format with little in the way of colors or visuals.

Users can access explanations for each pre-made framework via the “i” information button in the top right corner, which would be accessible via both mouse and keyboard hover. This is a standard icon which signifies tooltips or popup tips. [15] We envision that pedagogy researchers and other domain experts could assist eLC/Brightspace in coming up with premade frameworks for a solution that would be most useful to instructors. Of course, the current method of creating a custom grade schema/setup would still be available to instructors (which is shown in the wireframe’s “Framework Editor” screen).

Because the two ideas for this user story are similar, we felt that these ideas can be combined in a single wireframe.For example, the tile framework desgin refers to idea 1 and the explanations for which framework to use are part of idea 2, and these two ideas were combined in the public framework frame.

User Story 4
{% include_relative assets/html/figma/wireframe4.html %}
Justification:
We added a separate page from which instructors could add multiple categories for their class in bulk. This form page follows conventional design guidelines for data entry forms, such as providing clear visual delimiters of the form field boundaries, informative labels, and consistent spacing. [16] We believe the ability to add multiple at once is an improvement as it allows for quicker configuration.

We added a drag and drop interface to the Manage Grades Page’s Grade Item table. With the current eLC design, to change the category of a grade item, instructors must make several clicks on different pages. With this redesign, it would be much quicker and more intuitive to change the category. 

To indicate that the rows are draggable, we chose the six dots icon which is a common signifier in use for this purpose [17]. In addition, to further signal the intended behavior, we imagine that the cursor would change upon hovering over one of the rows to the platform standard for movement (a grabbing hand on Mac or crossbar on Windows), but we could not include that behavior in the wireframe. We included a drop shadow to provide feedback when an item is selected for dragging, which is also a standard signifier to let users know which item they are currently moving [17]. This same icon is used by Canvas, a market-leading LMS, for the same purpose of allowing instructors to reorganize grade items and their groups. [18]


User Story 5
{% include_relative assets/html/figma/wireframe5.html %}
Justification:
In these wireframes, we attempted to make the experience of adding a grade item as easy and simple as possible for instructors, with individual boxes for each important grade item field so instructors can more efficiently create understandable and informative grade items. 

We also included the warning for certain student-friendly features missing in a popup format in order to more easily bring to the attention of an instructor certain things which have been important to students when viewing the gradebook. [1] We felt this was the best design because the popup is more urgent and requires an extra action for the instructor to purposely omit certain items during grade item creation. Popups are great for bringing an item to a user’s attention but can be annyoing if overdone, so in our design we followed the recommended pattern of only showing the popup after a user action (clicking the save button if there is incomplete information). [19]


## C. Detailed Designs

Source Figma File:

User Story 1
{% include_relative assets/html/figma/mockup1.html %}
Justification:
In our high-fidelity mockup of a student’s eLC grades view, we chose the grade calculator idea to be the best, as it added more functionality which was currently missing. The idea of having a student’s final grade displayed by default did not in and of itself necessitate a design change on the student view end, unlike the grade calculator tool. But a grade calculator tool would be most useful if the current grade is made available to students, so we kept with the ideal that the overall grade would be displayed to students. Our research has led us to conclude that the combination of both of these design features would adequately address students’ current desires for the eLC (Desire2Learn) Grades view. Namely, this would address student concerns that “Gradebooks are not set up to display current course grade” and “Gradebooks are not set up to display final grade”. [1]

We carried over the decision made in our wireframes of this story, which was to continue with eLC’s existing functionality by displaying the final grade at the top of the grades table. We added the feature of a color which varies based on the letter grade or score bucket (determined by the instructor’s grade schema) for the final grade. We took this idea for this color signifier from Blackboard, which utilizes a similar system to highlight the grades with colors, corresponding with letter grades. [8] We feel that this additional signifier helps to indicate a student’s performance at a glance and would be helpful to include in our high-fidelity proposed solution.

Additionally, we kept with the decision to keep the grade calculator tool on the right hand side of the page, modeled after Canvas’s “What If” tool’s placement. [18] We also added the color signifiers to the Grade Calculator tool on the right.

User Story 2
{% include_relative assets/html/figma/mockup2.html %}
Justification:
For this story’s high fidelity mockup, we chose to incorporate both of our design ideas from the wireframes. Both ideas deal with different aspects of the user action of setting up the gradebook configuration, and as such, both are important to include in our proposed design.

We continued with the idea of adding more visuals by keeping the two-toned color progress bar at the top of the page to signify which sections of eLC an instructor is working on and how much is left. 

We also added a proper error/warning message in order to display that the instructor is attempting to move on without the prefered defaulted action. This allows instructors to be notified that the students will not have access to an important and recommended feature. The red text is typical in western cultures to convey a sense of warning and urgency, and we kept this color usage consistent throughout the other mockups as well. [20]

Blackboard, another LMS, has an appropriate use of icons and colors so we mirrored these for our redesigned eLC page as well. [8] This is accomplished through the additions of blue and green which we incorporated into the navigation buttons at the bottom of each page.


User Story 3
{% include_relative assets/html/figma/mockup3.html %}
Justification:
As this user story only had one series of actions in the wireframe that encompassed both design ideas, we did not have to pick between multiple design options. One change we have made from the wireframe was adding a red warning for when the weighs of the sections do not add up to 100. Red in western cultures often signifies urgency, which we felt this change would represent by requiring the user to make sufficient changes before finalizing them [20].

In addition, we made more use of colors where a heavier shade of blue indicates a heavier grade weight, whereas a lighter shade indicates a lighter grade weight. We decided to use blue for this case because blue was already being used in the hyperlink and button colors, and we did not want to bombard the user with multiple colors. As a result of better use of colors, we believe that the interface for our mockup becomes easier to use in contrast to the original eLC format, which was largely text based and had very few colors or graphics.

User Story 4
{% include_relative assets/html/figma/mockup4.html %}
Justification:
For our high fidelity mockup, we combined the two ideas of having a separate form page to add categories in bulk, and to provide a drag and drop interface to quickly change the categories of a grade item (or the order in which items/categories are displayed). The combination of the two design ideas provides the full range of activities encompassed by this user story, and so we felt that both ideas could be incorporated for the best solution.

We kept most of the design decisions made in the wireframe, such as which drag handle icon to use and the configuration of the new form to add categories.

One additional adjustment to the UI that was not included in the wireframe, was the decision to split out the “New” button into two separate buttons for “New Item” and “New Category”. We felt that this would be important because it reduces the number of clicks instructors need to make in order to add an item [21]. In addition, the new redesign for the “New Category” page makes it quite different to the “New Item” page, and because users are accomplishing two different goals with each option, it did not make much logical sense to group the buttons together. We wanted the “New Category” button to be immediately visible and accessible, to encourage instructors to make use of this grouping system.
Upon keyboard or mouse hover or active state, the buttons will turn a darker shade - such interaction mimics the behavior already found on eLC and helps indicate to a user that the button is selectable. [22]

User Story 5
{% include_relative assets/html/figma/mockup5.html %}
Justification: 
Again, we chose to incorporate both of our design ideas from the wireframes into our completed mockup of this user story. Both ideas deal with different aspects of the user action creating a grade item, and as such, both are important to include in our proposed design.

We changed the look of the warning popup message from the wireframe to the mockup. We used red font and icons for the warning message in order to be consistent with our other mockups, which also use red for warnings. Red in western cultures often signifies urgency, which we felt this change would represent by notifying the instructor they may have forgotten something when filling out the form [20]. We also switched the coloration of the buttons on the warning pop up to be blue for “Cancel” and grey for “Submit anyway” in order to indicate that “Cancel” is the primary/preferred option in this case. Finally, behind the error message, the fields which were either invalid or incomplete are highlighted in red, to more clearly bring it to the user’s attention.

We also added a final frame which shows the existing “Advanced Settings” options for instructors. The look of this frame is largely modeled after eLC’s existing design, and is important so that our high fidelity mockup includes all options that instructors have when creating a grade item. As this section is already well organized with font weights and colors, we did not need to make additional changes to the design.

Similar to Mockup 4, we carried over the decision to split out the “New” button into two separate buttons for “New Item” and “New Category”. We felt that this would be important because it reduces the number of clicks instructors need to make in order to add an item. [21] Upon keyboard or mouse hover or active state, the buttons will turn a darker shade - such interaction mimics the behavior already found on eLC and helps indicate to a user that the button is selectable, as can be seen in the first frame. [22]

## D. Summary Video
Link to video: <https://youtu.be/dZ1BWm1WqSg>

{% include_relative assets/html/youtubeMilestone3.html %}

## Sources

[1] Student Experience with D2L and other LMSs. University of Colorado Boulder. 2016. From <https://www.colorado.edu/lms/sites/default/files/attached-files/lms_eval-stud_1.pdf>

[2] LMS Evaluation and Selection Project Faculty Survey Report. University of Colorado Boulder. 2017. From <https://www.colorado.edu/lms/sites/default/files/attached-files/lms_eval-fac_0.pdf>

[3] Ben Shneiderman, Catherine Plaisant, Maxine Cohen, Steven Jacobs, Niklas Elmqvist, and Nicholas Diakopoulos. Chapter 3.3.4: The Eight Golden Rules of Interface Design. In Designing the User Interface. Pearson, Boston, 6 edition, 2017.

[4] Spreadsheet analyzing online sentiment of D2L, via reddit comments. <https://docs.google.com/spreadsheets/d/1k4ryR_frWc1d-duoLC8xsZjQlYNBuNmeGjvWkQCUQ2U/edit?usp=sharing>

[5] Grades Setup: Gradebook: Assessments: eLC Help. UGA. From <https://help.elc.uga.edu/assessments/gradebook/grades_setup/>

[6] Set up your grade book. Brightspace Help. 2021. D2L. From <https://documentation.brightspace.com/EN/le/grades/instructor/set_up_grade_book.htm>

[7] How do I use the Gradebook? Instructure Community. 2021. Instructure. From <https://community.canvaslms.com/t5/Instructor-Guide/How-do-I-use-the-Gradebook/ta-p/701>

[8] Navigate Grading. Blackboard Help (Instructor). 2021. Blackboard Inc. From <https://help.blackboard.com/Learn/Instructor/Ultra/Grade/Navigate_Grading>

[9] Instructure. How do I approximate my scores using the What-if tool? (2021). <https://community.canvaslms.com/t5/Student-Guide/How-do-I-approximate-my-assignment-scores-using-the-What-If/ta-p/481>

[10] Lindsay McKenzie. 2018. Canvas Catches, and Maybe Passes, Blackboard. Inside Higher Ed. <https://www.insidehighered.com/digital-learning/article/2018/07/10/canvas-catches-and-maybe-passes-blackboard-top-learning>

[11] De la Fuente, Juanma & Casasanto, Daniel & Santiago, Julio. (2014). Observed motor actions affect valence judgments. 36th Annual Conference of the Cognitive Science Society. <https://www.researchgate.net/publication/264311119_Observed_motor_actions_affect_valence_judgments> 

[12] Johnson, E.J., Bellman, S. & Lohse, G.L. Defaults, Framing and Privacy: Why Opting In-Opting Out1 . Marketing Letters 13, 5–15 (2002). <https://doi.org/10.1023/A:1015044207315>

[13] "Aspects of Smart Decision-Making". Handbook of Behavioural Economics and Smart Decision-Making: 155–156. (2017). doi:10.4337/9781782549598.00016.

[14] Nielson, Jacob. (2004). Checkboxes vs. Radio Buttons. Nielson Norman Group. <https://www.nngroup.com/articles/checkboxes-vs-radio-buttons/>

[15] Joyce, Alita. (2019). Tooltip guidelines. Nielson Norman Group. https://www.nngroup.com/articles/tooltip-guidelines/

[16] Sidney Smith, Jane Mosier. 1986. Guidelines for Designing User Interface Software. From http://www.hcibib.org/sam/1.html

[17] Laubheimer, Page. (2020). Drag-and-Drop: How to Design for Ease of Use.  Nielson Norman Group. https://www.nngroup.com/articles/drag-drop/

[18] Instructure. How do I move or reorder an assignment? (2021) https://community.canvaslms.com/t5/Instructor-Guide/How-do-I-move-or-reorder-an-assignment/ta-p/1289

[19] Kaley, Anna. (2019). Popups: 10 Problematic Trends and Alternatives. Nielson Norman Group. <https://www.nngroup.com/articles/popups/>

[20] Edward Wegman and Yasmin Said. Color theory and design. WIREs Computational Statistics, 3(2):104–117, 2011. doi:https://doi.org/10.1002/wics.146.

[21] Harley, Aurora. (2015). No More Pogo-Sticking: Protect Users From Wasted Clicks.  Nielson Norman Group.  https://www.nngroup.com/articles/pogo-sticking/

[22] Babich, Nick. (2018). 7 Basic Rules for Button Design. UX Planet. https://uxplanet.org/7-basic-rules-for-button-design-63dcdf5676b4

**BIT210 Group Assignment** 


**													

Release Date:			9<sup>th</sup> January 2025

Due Date:			10<sup>th</sup> February 2025 400pm (Malaysia time)

Value:				20% of total assessment

Marks:				Marked out of 100

Assessment Mode:		Group (2 students) and Individual Assessment
**



**RATIONALE**

This assignment has been designed to allow students to test and demonstrate their understanding and ability to implement HTML5, CSS, Angular and relevant libraries / frameworks to develop a front-end web application. On completion of this coursework, the student will be able to:

- CLO2: Evaluate the applications of different libraries, frameworks, and technologies in creating a web application.
- CLO3: Develop responsive and dynamic web applications using current technologies.







**CASE STUDY: Waste Management Web Application**

Waste management is a significant problem in Malaysia as waste output outpaces the country’s recycling rate. Malaysia disposes of more than 30,000 tons of municipal solid waste (MSW) daily, which amounts to 1.17kg of waste daily per capita. Food waste contributed the most significant component of MSW, followed by plastic, paper, mixed organic, wood, and others (Market Intelligence, 2022).

Malaysia is heavily dependent on landfilling as a method of waste disposal, and as a result, severe space constraints, health issues, and environmental issues will eventually affect the country.  Local environmental experts have forecasted no space will be available by 2050 if nothing is done to reduce waste (Market Intelligence, 2022). In Malaysia, households are the main producers of municipal solid waste, with recyclable materials making up between 70 and 80 percent of the total waste found in landfills.

It was reported that Malaysia loses an estimated RM476 million every year in recyclable resources in an industry that is considered to have high value, simply because recycling practices have yet to become the norm in this country (NST, March 2023).

Community participation and education can significantly improve solid waste management and health outcomes by actively engaging community members in the entire waste management process.  









**REQUIREMENTS**

<a name="_hlk155534878"></a>Develop a waste management system to streamline and improve waste collection and disposal processes for a community. This proposed system ensures the proper collection, treatment, and disposal of waste, reducing environmental pollution and health hazards. Effective waste management also promotes recycling and resource recovery, resulting in cleaner environments and healthier populations.

You are required to design for implementation as either a web or mobile application. The system encompasses six use cases, each addressing essential aspects of community waste management (refer to Fig. 1).

![A diagram of a diagram

Description automatically generated](Aspose.Words.ba08e822-68fa-48e8-afd2-7f072a97b303.001.png)














Fig. 1: CWMS Use Case Diagram
**


**HIGH LEVEL USE CASES**

- **Manage Users Use Case**

  Users can create accounts and securely log in to access personalized features. This foundational use case ensures that each community member can have a unique profile, enabling the system to provide tailored services and notifications. Users are part of a community; thus, a community needs to be registered before the community users.

- **Schedule Waste Pickup Use Case**

  Community members can schedule waste pickups by selecting the type of waste and their preferred date and time. This feature helps coordinate efficient waste collection, reducing missed pickups and optimizing route planning for the waste collection team.

- **Report Issues Use Case**

  Users can report waste management issues such as missed pickups, overflowing bins, or illegal dumping. This use case empowers the community to communicate problems directly to the administrator, facilitating quicker resolutions and maintaining cleanliness.

- **View Pickup History Use Case**

  Users can access a history of their past waste pickups, including dates and types of waste collected. This transparency helps users keep track of their waste disposal habits.

- **Manage Notifications Use Case**

  The system sends notifications to users about upcoming scheduled pickups, reminders to schedule a pickup, and important community announcements. This feature keeps users informed and engaged, promoting timely waste disposal and community participation.

- **Generate Reports Use Case**

  Both users and the admin can generate reports on various metrics such as pickup statistics, reported issues, and recycling rates. These reports provide valuable insights into the effectiveness of the waste management process and help identify areas for improvement.

**EXPANDED USE CASES**

|Use Case 1|**Manage Users**||
| :- | :- | :- |
|Goal in Context|The goal of this use case is to enable community members to register for an account and log in to the system to access personalized waste management features.||
|Primary Actor |<p>Community members (users)</p><p>Community Admin (representative of the Community)</p><p></p>||
|Trigger |A registered user wants to access the personalized waste management services.||
|**Typical Course of Events**|||
|**Actor Action** |**System Response**||
|1. This use case begins when the user initiates the profile creation (sign up)/sign in process.|2. The app displays the appropriate user profile interface.||
|3. User inputs or updates their personal details in the respective profile fields. The user fills in the full name, contact number, email, community name, residential address. |4. The system saves the record into database after validating all user inputs. The system will generate a login with the user email and a default password sent via the email address.||
|**Alternative Course of Events**|||
|<p>Line1a: Successful login will redirect to the user’s dashboard.</p><p></p><p>Line 3a: If the username/email had been registered by other user, the system will prompt a message to remind the users.</p><p></p><p>Line 3b: If the community is not listed, the community administrator enters the community’s name and the general address, and the waste pickup times in term of days and time for the community. A single admin for each community. </p><p></p>|||



|Use Case 2|**Schedule Waste Pickup**||
| :- | :- | :- |
|Goal in Context|The goal of this use case is to enable community members to schedule waste pickups by selecting a date and type of waste.||
|Primary Actor |Community Users||
|Trigger |A community member wants to schedule a waste pickup.||
|**Typical Course of Events**|||
|**Actor Action** |**System Response**||
|1. The user opens the application and logs in with their credentials.|2. A successful login will redirect the user’s dashboard.||
|3. The user selects the "Schedule Pickup" option from the dashboard or main menu.|4. The community scheduled days and times are shown as specific dates ||
|5. The user selects a preferred date and time for the waste pickup based on the generic waste pick up time.|6. The system confirms the appointment by storing the residential address that requests the waste pickup. ||
|7. The user chooses the type of waste they want to dispose of (e.g., household waste, recyclable waste – paper/plastic/aluminium etc, hazardous waste).|8. The system will store the types of waste which is requested for the pickup. The user will receive a confirmation message with details of the scheduled pickup.||
|**Alternative Course of Events**|||
|7a. If the user does not specify the type of waste, the system prompts them to select at least one option.|||





|Use Case 3|<h3>**Report Issues**</h3>||
| :- | :- | :- |
|Goal in Context|To enable community members to report issues related to waste management, such as missed pickups or overflowing bins.||
|Primary Actor |Community members (users)||
|Trigger |A community member encounters an issue with waste management and wants to report it.||
|**Typical Course of Events**|||
|**Actor Action** |**System Response**||
|1. The user opens the application and logs in with their credentials.|2. The app collects and analyses the user's historical activity data, considering factors such as transportation habits, energy consumption, and dietary choices.||
|3. The user selects the "Report Issues" option from the dashboard.|4. The app displays the form to enter the details of the issues. ||
|5. The user chooses the type of issue they want to report (e.g., missed pickup, overflowing bin, illegal dumping) and enters the details of the issue, such as location, description and any additional comments and photos if possible. |6. The system validates the information provided by the user. The system logs the issue in the database with a unique issueID. Status of the issue will set to NEW.||
|7. The user receives a notification that includes a confirmation message that their issue has been reported successfully. The message includes the unique issue ID and status.|||
|**Alternative Course of Events**|||
|<p>5a. If the user does not specify the type of issue, the system prompts them to select an option.</p><p>5b. If the user provides insufficient details, the system prompts them to enter the required information.</p>|||



|Use Case 4|**View Pickup History**||
| :- | :- | :- |
|Goal in Context|Users can access a history of their past waste pickups, including dates and types of waste collected. This transparency helps users keep track of their waste disposal habits and ensures accountability from the waste collection team.||
|Primary Actor |Community members (users)||
|Trigger |A community member wants to review their past waste disposal activities.||
|**Typical Course of Events**|||
|**Actor Action** |**System Response**||
|1. User logs in using their credentials.|2. System authenticates the user.||
|3. User navigates to the "Pickup History" section in the dashboard.|4. The system retrieves and displays a list of past waste pickups for the user. The list includes dates, types of waste collected, and any other relevant details.||
|5. The user can apply filters (e.g., date range, type of waste) to narrow down the list. The user can sort the list by date, type of waste.|6. System displays using suitable charts and tables.||
|**Alternative Course of Events**|||
|<p>3a. If no pickup history is available for the user, the system displays a message indicating that no pickups have been recorded.</p><p>5a. If the user applies filters that return no results, the system displays a message indicating   that no pickups match the selected criteria.</p>|||



|Use Case 5|**Manage Notifications**||
| :- | :- | :- |
|Goal in Context|To provide users with timely notifications about upcoming scheduled pickups, reminders, and important community announcements related to waste management.||
|Primary Actor |<p>Community members (users)</p><p>Community Admin (representative of the Community)</p>||
|Trigger |A scheduled event that warrants a notification, such as an upcoming waste pickup or a community announcement.||
|**Typical Course of Events**|||
|**Actor Action** |**System Response**||
|1. User logs in using their credentials.|2. System authenticates the user.||
|3. User receives the notification. User can view the details of the notification.|4. The system generates a notification message containing relevant details about the event.||
|**Alternative Course of Events**|||
|3a. Admin can broadcast community announcements.|||








|Use Case 6|**Generate Reports**||
| :- | :- | :- |
|Goal in Context|To enable users and the admin to generate reports on various aspects of waste management, such as pickup statistics, issues reported, and recycling rates.||
|Primary Actor |<p>Community members (users)</p><p>Community Admin (representative of the Community)</p>||
|Trigger |A user or admin initiates a request to generate a report.||
|**Typical Course of Events**|||
|**Actor Action** |**System Response**||
|1. User logs in using their credentials.|2. System authenticates the user.||
|3. The user selects the "Reports" option from the dashboard.|4. System to display a generic report and allow user to choose the type of reports to be generated.||
|5. The user chooses the type of report they want to generate (e.g., pickup statistics, issues reported, recycling rates). The user specifies parameters for the report, such as date range, type of waste, or specific areas within the community.|6. Report is generated based on the specified parameters using graphs and tables.||
|**Alternative Course of Events**|||
|5a. If there is insufficient data to generate the report, the system displays a message indicating the lack of data and suggests alternative parameters or date ranges.|||









**Additional Information:**

- Please develop this system using Javascript front end framework.

- You are not allowed to use any content management system such as Joomla, WordPress, Drupal, or any other similar platform for this assignment. You can use code editor such as Visual Studio to do it.


**TASKS**

Produce a project report. Your report MUST include the following points:

1. Project Title.
1. Table Content of the report.
1. List all the technologies, frameworks, and libraries used to build this web application. Justify the choice of technologies with support from exiting literatures.
1. Manual guide of web setting / configuration / installation of node JS and packages required to execute the application.
1. User manuals of the web application that you developed (Individual and Group functionalities).
1. Create a video to present your prototype in a user manuals way.
1. List out all references that are used in APA format. 


**SUBMISSION CHECK LIST**

1. Upload the project source code to the HLMS link provided.
1. Upload the project report in Word document to the HLMS link provided.
1. Only one submission is allowed.




**REMARKS**

1. This assignment should be prepared using word processing software with 12 points Times New Roman font, 1.5 spacing, and page numbering.
1. If you are not clear about the assignment requirements, please contact the module leader.
1. You may refer to materials from textbooks or any other references, but you must acknowledge the quotation, no matter how brief. Failure to do so will result in zero marks being awarded for the assignment.
1. All assignments should be accompanied by a completed assignment cover sheet. **You must sign the submission form during your submission.**
1. A penalty of 5 marks per working day (including Saturday) deduction from the marks obtained for this assignment will be imposed for late submission.
1. If students are not able to submit any item in the checklist, students will be awarded 0 mark for this assignment for all group members.

















|<a name="_hlk140841502"></a>**Use of AI generative tools**|<p>1. Utilizing AI generative tools should be seen to augment creativity, problem-solving, and productivity while maintaining the integrity of the subject matter and upholding academic and professional standards.</p><p>&emsp;</p><p>2. Students must demonstrate their own knowledge, skills, and understanding of the subject matter in their work.</p><p>&emsp;</p><p>3. Where an assignment requires ChatGPT to be cited, you must reference all the content from Generative AI tools that you include. Failure to reference externally sourced, non-original work can result in Academic misconduct.</p><p>&emsp;</p><p>4. Students are to apply **APA Style** for any AI content generated that is utilized and integrated into the final work. This acknowledgment is to be added to the **footnote** of the respective pages.</p><p></p><p>- **To cite AI-generated work that you did not edit or revise:** </p><p>&emsp;Name of AI Tool. (Year, Month Day you generated the content). Exact text of question or prompt you entered [AI-generated text/image/video, etc.]. Name of Company/Developer if different than name of AI tool. URL. </p><p>&emsp;Example: ChatGPT. (2023, June 3). “Steps of creating a running website using XAMPP?” [AIgenerated text]. OpenAI. <https://chat.openai.com>. </p><p>&emsp;</p><p>- **To cite AI-generated work that you edited or revised:** </p><p>&emsp;Name of AI Tool & Your Last Name, First Initial. (Year, Month Day you generated the content). Exact text of question or prompt you entered [AI-generated text/image/video, etc.]. Name of Company/Developer if different than name of AI tool. URL. </p><p>&emsp;Example: ChatGPT & Chong, L.Y. (2023, July 19). How to setup cloud based CI/CD for a website deployment? [AI-generated text]. OpenAI. https://chat.openai.com/c/9bb6771b-209b-4c8c-ac79-6a8a9f39604a   </p><p>- **General Format for In-Text Citations**  </p><p>&emsp;Examples: To make fluffy basmati rice, “rinse the rice twice in cold water” (ChatGPT, 2023) </p><p>&emsp;Cloud-based CI/CD requires the following steps to be applied (ChatGPT & Chong, L.Y., 2023)</p><p>5. Any violation of this policy will result in appropriate academic sanctions, which may include penalizing your grades, failing the course, and other disciplinary actions.</p>|
| :- | - |


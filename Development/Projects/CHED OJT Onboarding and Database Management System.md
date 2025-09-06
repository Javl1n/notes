# CHED OJT Onboarding and Database Management System For CHED Regional 12: Laravel Framework
Purpose:
para mag onboard sa mga ojt, mag give information sa ila about sa ched, attendance, task management for ojt and database listing with performance
## Features
1. Information Dissemination
	- feature where ojt students can view information about CHED, their roles, departments, etc. ma edit din siya sa admin through markdown.
2. Ojt Attendance Tracking
	- Attendance for ched sa mga ojt, para ma track nila kung unsa oras ga time in ang ojt, time in time out, either sa computer sa admin or something, depende pa kung online ba ni or local lang ila system
3. Task Management
	- Where admin can give tasks to ojts through the system, mura siyag todo list or ojt journal sa mga ojt, pwede pud sila ka add ug mga todo nila mismo para matrack ilang progress 
4. Performance Tracking
	- summary sa attendance ug task management, diri ma kita ang performance sa ga ojt, nya pwede pud maka hatag ang admin ug rating base sa ilang impression sa student, and database napud ni siya para if ever mangapply ang student sa ched inig graduate, naa na silay record sa CHED
5. Announcements and Notification
	- kung asa ang admin maka send ug announcements sa mga ojt. pwede ni ichange na chatting lang kung prefer sa CHED.

## Features after Defense 
1. Information Dissemination
	- functions in different offices
	- Can add video and pictures
	- embed to youtube
2. Task Management 
	- Removed
3. Time In and Time Out 
	- without journal
	- summary for a week
4. Performance Management - Performance Rating
	- Sali sa rating sheets
	- performance rating
	- subjective
	- self assessment
		- before and after
	- Evaluation of Supervisor to OJT
	- OJT to the Supervisor
		- annonymous only viewed to the admin
5. Announcemnt
	- Sali sa onboarding
6. Chat 
	- removed
7. Profiling
	- import / export profiling
	- not really necessary, simple lang for information
	- dynamic field - add year
	- demographic profile
8. Report Generation
	- List of Clients
	- Monthly, Daily,  Reports
	- Rating and Profile
## Features
1. Information Onboarding
	- uses markdown format so that the admin can edit the information, can add pictures, embed youtube video or google drive
	- gather videos
2. OJT Time In and Time Out
	- Daily Time in feature
	- add weekly summaries, every Friday
3. Performance Rating
	- OJT
		- have self assessment before and after their OJT period
		- give feedback to their Supervisor, anonymously or only admin can view
	- Supervisor
		- give feedback to OJTs
	- Admin
		- View feed backs to supervisors
		- Manage assessment questions
4. Profiling
	- Export Profiling Data, either in excel or csv or json format
	- OJT account registration process:
		- register account
		- wait for verification
		- admin reviews the user
			- get data from profiling database
		- ojt can check if they are verified if they log in to their account again
	- Add Academic Year and Semester for future proofing
	- Demographic Profile
5. Report Generation
	- Summarize report on the OJT
	- weekly, monthly, etc.
	- (possible) use ai for generative report summary

## akong i ask kay kaye
- unsa ang mga klase klase nga departments sa CHED... naa bay kalahian ang isa isa sa ila na unique?
- ma view ba sa tanan ojt ang information sa tanan department or specific lang sa ila?
- di nako klaro ang report generation na ilang gi mention, unsa ang process sa report generation?
- Kinsa ang mga supervisor? head sa department or naay naka assign sa inyo na mag supervise?
- Online ni? or ma access lang within the CHED?
- Naa baya jud ni maintenance cost, pricing sa hosting, sa apis if naay gamiton, I think sila jud dapat mu cover ani nga cost kay sila may mugamit
- pwede mag integrate ai? like for example naay ai summarization sa reports

# Site Map
## OJT
- Time in / Time Out Button
	- Direct button, no page
- About CHED (Onboarding)
	- CHED
	- Departments
- Assessment
	- Self Assessment
		- Only viewed at the start and end of semester
	- Supervisor Assessment
		- At the end of Semester
		- Can add a weekly report about the supervisor, text input only
## Supervisor
- Dashboard
	- Table for when OJTs that they supervise has timed in or out
	- each row directs to OJT Profile Page
- OJT Profile
	-  View OJT Profile, weekly assessments, self assessment, time in and out history
	- can add a weekly report about the OJT
- Onboarding
	- CHED and Departments
	- Can edit only their own department
## Admin
- OJTs
	- Table for when OJTs has timed in or out
	- Can Export button
- OJT Profile
	- profile, weekly assessments, self assessments, reports, average time in and out, including history, reports to supervisor
- Onboarding
	- CHED and Departments
	- Can edit all departments
	- add department
- Supervisors
	- profile, assessments of students for them
	- add supervisor
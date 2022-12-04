Project: Meeting Management Application

Project Description: 
This Application can be a tool used to send out meeting invitations to the participants as well as send them reminders before the meeting. The team leads can set up meetings with their teams. Furthermore, it will keep track of which participants were invited, who accepted, and who rejected the meeting invitation.

Documentation Requirements:

There shall be user manuals with instructions to help users learn to use the application
There shall be installation documentation that covers the prerequisites as well as the process of installing the application.
There shall be developer documentation to help the developers understand where to contribute to the code and how to review the changes 
There shall be a README.MD file with all the important instructions needed for the project.

Security Requirements:
The system shall have authentication measures at all entry points so that only the logged-in users can access the data.
The user accounts shall have limited privileges. Only the team leads will have the privilege to add or remove team members and view their meeting history. 
The system shall lock an account to protect a user's information from potential hackers after a specific number of login attempts
The system shall not sign up a user until the user creates a strong password. For example, a strong password might contain a certain number of characters and a capital letter.
The system shall Only the users with the role “site admin” to view the applicant’s personal information and edit them

Reliability Requirements:
The system shall apply load balancing 
The system shall perform without failure in 90 percent of use cases during a month.
The system shall allow applicants to resume their access 98% of the time without failure.
Performance Requirements:

System must load all pages in 2 seconds.
Hardware should be compatible with the application
The system shall give the last remainder at an appropriate time.
 The system shall keep record of traffic and  the shortest route to reach the destination.
The system shall be able to run with 3G , 4G or later technologies in mobile phones and should also operate on any wifi.
 The system shall be able to support 1000 simultaneous users.
Database performance should be optimised.
Contention(Contention is the condition in which two or more components of the workload are attempting to use a single resource in a conflicting way) should not increase the required limit. Contention increases then throughput decreases
If the number of users of a website increases then it should give bandwidth limited messages.
If a major incident happens on the application, the business must take measures to go back to being fully operational within a few days.
The application should update the users with the ongoing traffic situation as soon as any changes occur.
The notifications/ reminder should be given to the users on exact time, delay can cause error
The application should support different environments like Android, iOs etc


Modularity Requirements
The application need to be homogeneous both for iOS and Android
A native core module should be developed, which addresses needs common to all modules, and includes networking, internal and analytics events, security, dependencies injection, feature flag management etc.
Feature Flags should be used, they allow to turn off module functionality at run time.
Interdependencies should be avoided.
Coupling should be less.
 System shall integrate properly with google maps and google calendar
 A module’s implementation should be flexible enough that any change can be made without affecting any of the module’s users

 

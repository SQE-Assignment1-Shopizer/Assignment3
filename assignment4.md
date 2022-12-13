## Project: Meeting Management Application

### Project Description: 
This Application can be a tool used to send out meeting invitations to the participants as well as send them reminders before the meeting. The team leads can set up meetings with their teams. Furthermore, it will keep track of which participants were invited, who accepted, and who rejected the meeting invitation.

### Documentation Requirements:

1. There shall be user manuals with instructions to help users learn to use the application
2. There shall be installation documentation that covers the prerequisites as well as the process of installing the application.
3. There shall be developer documentation to help the developers understand where to contribute to the code and how to review the changes 
4. There shall be a README.MD file with all the important instructions needed for the project.

### Security Requirements:
1. The system shall have authentication measures at all entry points so that only the logged-in users can access the data.
2. The user accounts shall have limited privileges. Only the team leads will have the privilege to add or remove team members and view their meeting history. 
3. The system shall lock an account to protect a user's information from potential hackers after a specific number of login attempts
4. The system shall not sign up a user until the user creates a strong password. For example, a strong password might contain a certain number of characters and a capital letter.
5. The system shall Only the users with the role “site admin” to view the applicant’s personal information and edit them

### Reliability Requirements:
1. The system shall apply load balancing 
2. The system shall perform without failure in 90 percent of use cases during a month.
3. The system shall allow applicants to resume their access 98% of the time without failure.


### Performance Requirements: 
1. System must load all pages in 2 seconds.
2. Hardware should be compatible with the application // -iuhi
3. The system shall give the last remainder at an appropriate time.
4. The system shall keep record of traffic and  the shortest route to reach the destination.//
5. The system shall be able to run with 3G , 4G or later technologies in mobile phones and should also operate on any wifi.
6. The system shall be able to support 1000 simultaneous users.
7. Database performance should be optimised.
8. Contention(Contention is the condition in which two or more components of the workload are attempting to use a single resource in a conflicting way) should not increase the required limit. Contention increases then throughput decreases
9. If the number of users of a website increases then it should give bandwidth limited messages//.
10. If a major incident happens on the application, the business must take measures to go back to being fully operational within a few days.
11. The application should update the users with the ongoing traffic situation as soon as any changes occur.
12. The notifications/ reminder should be given to the users on exact time, delay can cause error
13. The application should support different environments like Android, iOs etc


### Modularity Requirements
1. The application need to be homogeneous both for iOS and Android
2. A native core module should be developed, which addresses needs common to all modules, and includes networking, internal and analytics events, security, dependencies injection, feature flag management etc.
3. Feature Flags should be used, they allow to turn off module functionality at run time.
4. Interdependencies should be avoided.
5. Coupling should be less.
6. System shall integrate properly with google maps and google calendar
7. A module’s implementation should be flexible enough that any change can be made without affecting any of the module’s users

 

### Process Requirements
1. SCRUM Framework shall be used for the development of this Application
2. Daily Meetings shall be scheduled with the stakeholders
3. Scrum Master shall keep track that everyone is on track
4. After a Sprint feedback shall be taken from stakeholders
5. A Product Backlog shall be maintained
6. All tasks shall be managed on Jira
7. Repositories shall be maintained on Github
8. Acceptance Test Driven Developement Practice shall be followed
9. Quality Assurance should be done through out the development




### UI, Unit and API Test Automation Framework Requirements
1. The purpose of the API shall be defined
2. Interactions with other APIS’s shall be defined
3. Behaviour of the API shall be defined
4. Input Parameters shall be defined
5. API Test cases shall be made
6. Eggplant Automation framework shall be used for API and UI testing
7. The Test Environment device shall have 2 GHz processor, 2 GB RAM, 1 GB free hard disk space for the installation of Eggplant
8. To run Eggplant  Studio, Test Controller, Analyzer, or the C# engine, Microsoft .NET 4.5 must be installed.
9. EggPlant shall be integrated with Jira
10. EggPlant DAI integration tool shall be used to launch DAI tests from within a GitHub workflow pipeline.
11. Test scripts shall be maintained
12. You shall be aware of the code versioning used in your Git repository.
13. Unit Tests shall be deterministic
14. Tests shall be named properly








# React Project - Part A

## Group Members

- Mill Daulagala
- Maurice Yong
- Rashid Elhouli
- Ashley Tsai

## Questionnaire

1. Who is your client?
    - Simon Cook from Encode Talent. He is a recruitment principle who runs his own company and focuses on candidate side more than client side.

2. What is your client’s need (i.e. challenge) that you will be addressing in your project?

    - A major part of his work is dealing with candidates via phone calls, where he runs an extensive questionnaire to get as much information about them possible. He spends 75% of his time on the phone and documents all his data manually in his notebook.
    - He has reached out to us to set up an online solution where he can get the candidates to fill out the questionnaire online and he can then view this once they submit it

3. Describe the client’s current setup and data.
    - He is currently documenting all his data in his notebook and then manually entering the data into an excel spreadsheet.

4. Describe the project will you be conducting and how your App will address the client’s needs.

    - We will build an online solution. The app will feature a questionnaire that his candidates can fill out. He can view all their responses once they submit. He will have a database of all the candidates who submitted the questionnaire and will able to filter through them accodrding to his needs. This will dramatically reduce the amount of time used for phone calls and help him better keep track of all his clients.

5. Identify and describe the software (including databases) to be used in your App.

    - VS Code
    - Figma
    - Trello
    - Slack
    - MongoDB

6. Identify and describe the network setup you will use in your development.

    - literally whether it's across the internet/connections to other services, etc

7. Identify and describe the infrastructure (i.e. hardware) that your App will run on.

    - what type of cloud service (AWS, google cloud), mongo atlas, etc.

8. Describe the architecture of your App.

    - flow and structures of the app

9. Explain the different high-level components (abstractions) in your App.

    - basic summary of major components (candidate, admin, etc)

10. Detail any third party services that your App will use.

    - literally any platform, cloud service, host, frameworks that we are using...

11. Identify the database to be used in your app and provide a justification for your choice.

    - We will be using MongoDB as the main database for storing candidate information, because ......

12. Discuss the database relations to be implemented.

    - candidate collection

13. Provide your database schema design.

    - could be a simple drawing chart

14. Provide User stories for your App.

    - **screenshot to Trello & link**

15. Provide Wireframes for your App.

    - **screenshot to lucidchart**

16. Describe the way Tasks are being allocated and tracked in your project.

    - Trello will be utilised to track progress on tasks and sprints, with each team member being responsible for their own delegated tasks
    - Morning stand-up meetings will also be held regularly to keep team members accountable to one another and tasks can be re-assigned and re-prioritised based on how tasks are progressing

17. Discuss how Agile methodology is being implemented in your App.

    1. We will be consulting with our client regularly during development to ensure that his expectations are met
    2. Should there be any change in requirements we will discuss and implement if it is feasible and keeps us on schedule
    3. New working functions/features are to be delivered by the end of each sprint to be incorporated into the app -- this is the main way that we will be measuring our project's progress
    4. The team will work in a self-organized manner, regularly meeting to discuss progress and provide support to one another, while also working self-sufficiently whether in pairs or individually. Tasks can be adjusted accordingly to improve efficiency and effectiveness

18. Provide an overview and description of your Source control process.

    - We will be using git as our primary version control system to track file changes during the development process. GitHub is the online service by which we will host our code and manage a central repository for the project, to which the team can make pull requests to update and make changes to the code.

19. Provide an overview and description of your Testing process.

    - Due to the time constraints given for the project, we are unable to incorporate a fully test driven development scheme. However, tests will be written for functional client-end components to ensure that features built for client interaction work. We will be utilising Jest as our testing framework for its simplicity and speedy performance.

20. Discuss and analyse requirements related to information system security.

21. Discuss methods you will use to protect information and data.

    - Users accessing the public form may only be able to post their personal information to the app, and not retrieve any personal information
    - User information and data will be stored securely in a MongoDB's Atlas platform, utilising their Salted Challenge Response Authentication Mechanism (SCRAM)
    - This information and data will be accessible through the app only by authorised users from Encode Talent who will need to be authenticated (email and password) to use the app

22. Research what your legal obligations are in relation to handling user data.

    - In accordance with Australia's *Privacy Act* 1988 we will be protecting our user's private information by storing them securely in a database and only allowing authorised users (our client - Encode Talent) to access user information for their recruitment activities
    - The candidates who will be submitting their personal information to the app will be notified of Encode Talent's privacy policy prior to the solicited collection of their information, to which they will consent to
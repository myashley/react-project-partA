# React Project - Part A

## Group Members

- Mill Daulagala
- Maurice Yong
- Rashid Elhouli
- Ashley Tsai

## Questionnaire

1. Who is your client?
    - Simon Cook from Encode Talent. He is a recruitment principal who runs his own recruitment company in the tech industry with emphasis on understanding his candidates' (people looking for work) qualities, career goals and aspirations before matching them with clients (employers seeking employees)

2. What is your client’s need (i.e. challenge) that you will be addressing in your project?

    - A major part of his work is dealing with candidates via phone calls, where he runs an extensive questionnaire to get as much information about them as possible. He spends 75% of his time on the phone and documents all his data manually in his notebook.
    - He has reached out to us to set up an online solution where he can get the candidates to fill out the questionnaire online and he can then view this once they submit it.

3. Describe the client’s current setup and data.
    - Candidates initiate contact with Simon via email or LinkedIn with an expression of interest
    - Simon then contacts candidates and carries out an initial interview (over phone or in person) with set questions to find out more about who they are, and their needs
    - He currently documents all his data in a notebook and then manually enters the data into an Excel spreadsheet
    - Relying on a combination of Excel, Hubspot, written notes and his own memory, he matches candidates with clients, conducting further meetings to gather more information from candidates if necessary

4. Describe the project will you be conducting and how your App will address the client’s needs.

    - We will build an online solution. The app will feature a questionnaire that his candidates can fill out. He can view all their responses once they submit. He will have a database of all the candidates who submitted the questionnaire and will able to filter through them accodrding to his needs. This will dramatically reduce the amount of time used for phone calls and help him better keep track of all his clients.

5. Identify and describe the software (including databases) to be used in your App.

    - We will use Node.js as a runtime environment to build this app, and use React as our JavaScript library/framework to develop our frontend. We will also use Express framework for our backend, and connecting to MongoDB database by using Mongoose as our driver.

6. Identify and describe the network setup you will use in your development.

    - The application will be deployed for use via the internet, with all users (candidates and admin) connecting to the application online through a networked device of their choosing (phone, tablet, PC, etc)
    - We will be connecting our servers to Now during development, and connecting to GitHub for group contribution.
    - The app will have its frontend server using Netlify for production and connecting to its backend server at Now.
    - The backend server connects to Mongo database by using MongoDB Atlas as its platform.
    - We plan on being able to utilise Encode Talent's existing domain and pointing to our application from a sub-domain

7. Identify and describe the infrastructure (i.e. hardware) that your App will run on.

    - The app will be accessed via web browser, which may be run from different devices such as mobile phones, tablets or computers.
    - The app will have its front-end and back-end sitting on different servers, using services including Now, Netlify and cloud services such as AWS or Google Cloud via Mongo Atlas.

8. Describe the architecture of your App.

    Below is the workflow digrams for our app. These highlight the different paths the candidates and admins take to use the app.

     ![workflow diagram](/assets/img/workflow.png)

9. Explain the different high-level components (abstractions) in your App.

    - The app consists of two major components: candidates and admininstrator. The candidate information will be collected, validated and stored into the database, and the administrator will be able to access the data for further management and manipulation.

10. Detail any third party services that your App will use.

    - The app will use Netlify and Now for its frontend and backend hosting, and use MongoDB Altas as the platform to manage MongoDB, which will be either hosted at AWS or Google Cloud.
    - The app will use React and Express as its JavaScript library and framework, using Node.js as its runtime environment.

11. Identify the database to be used in your app and provide a justification for your choice.

    - We will be using MongoDB as the main database for storing candidate information, because Structure of a single object is clear.
    - MongoDB is a document database in which one collection holds different documents. MongoDB doesn't have complex joins.
    - MongoDB has Deep query-ability and It supports dynamic queries on documents using a document-based query language.
    - The advantage of using MongoDB is we don't need to map application objects to database objects.
    - MongoDB store Data in the form of JSON style documents.

12. Discuss the database relations to be implemented.

    - The database is simple, with a candidate collection used to store individual candidate documents collected from candidate form submissions. There will also be a collection for user authentication (there will primarily be just one user -- our client) for access to the candidate data from client-side
    - These collections have no reference to one another, but user(s) may only access candidate information when they are authenticated via the application
    - A nice-to-have feature that we decided would be hard to implement within the timeframe of the project was for our client to be able to implement their clients (companies looking for candidates) as a collection with reference to the candidate data so that candidates could be short-listed to specific companies, however due to the time constraints, we decided that this would be a feature for further implementation in the future, hence there are no relations/references in our database

13. Provide your database schema design.

    ![Screenshot of Database Schema](assets/img/db_schema.png)

14. Provide User stories for your App.

    [Link to Trello](https://trello.com/b/v3SlV6aZ)

    ![Screenshot of User Stories](assets/img/user_stories.png)

15. Provide Wireframes for your App.

    [Link to Figma](https://www.figma.com/file/FyYzMMwDQTa4StkPC1kPjeiP/App-Design)

    *Candidate Form (Mobile)*
    ![Screenshot of candidate form (mobile)](assets/img/mobile_form.png)

    *Candidate Form (Desktop)*
    ![Screenshot of candidate form (desktop)](assets/img/desktop_form.png)

    *Admin Reports Dashboard (Mobile)*
    ![Screenshot of admin dashboard (mobile)](assets/img/mobile_admin.png)

    *Admin Reports Dashboard (Desktop)*
    ![Screenshot of admin dashboard (desktop)](assets/img/desktop_admin.png)

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

    - It is very important to protect the candidates personal information from potential threats.
    - In order to prevent unauthorized access, use, disclosure, disruption, modification, inspection, recording or destruction of information we will be implementing a secure Authorization process.
    - The implementation will include User authentication and User authorization.
    - The communication protocol will be HTTPS(HTTP Secure) for secure communication over a computer network.
    - For our specific requirements, only our client, as the main recruitment principal of his company, will have access to candidate data, and hence will be for now, the sole user of the application authorised to access, view and modify candidate data through our authentication system.

21. Discuss methods you will use to protect information and data.

    - Users accessing the public form may only be able to post their personal information to the app, and not retrieve any personal information
    - User information and data will be stored securely in a MongoDB's Atlas platform, utilising their Salted Challenge Response Authentication Mechanism (SCRAM)
    - This information and data will be accessible through the app only by authorised users from Encode Talent who will need to be authenticated (email and password) to use the app

22. Research what your legal obligations are in relation to handling user data.

    - In accordance with Australia's *Privacy Act* 1988 we will be protecting our user's private information by storing them securely in a database and only allowing authorised users (our client - Encode Talent) to access user information for their recruitment activities
    - The candidates who will be submitting their personal information to the app will be notified of Encode Talent's privacy policy and asked for consent prior to the solicited collection of their information
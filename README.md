# WebChat
## Idea 

When customers click on those chatbot apps they want to get a quick answer. Webchat allows your customers to add some basic information so that you know who they are and you can reach out to them. Webchat lets you keep track and assign conversations so that the conversation doesn’t get lost. Most importantly, Webchat is mobile ready so that users can ask questions and respond on their phones. 


### Mission statement:

Provide businesses with a streamlined workflow for managing and handling support requests, and provide their customers with a personable and conversational support  experience.


## User Journey

Caitlyn is the head of client success for a small company in Baltimore. They have clients all over the world visit their website. For years support requests have been sent via an email address. And then they get added to a ticketing system. Customers are given “support ticket number”. She hates it. Customers hate it. It doesn’t feel like a wonderful brand experience. She wants customers to feel like they have a direct line and an open conversation. Thanks to WebChat when a customer asks a question they get added to a shared queue with all of the client success reps. In the Webchat interface reps can have a live chat conversation with customers. Customers have a better experience, and conversations are handled better.

Gabe is a client success rep. He used to have a number of tools to manage messaging customers. He would switch from email to task manager and other collaboration tools. It was hard to make sure everyone knew who had responded to which customer and he was always worried he would make a mistake and risk his job. Thanks to Webchat Gabe and the other client success reps have a feed of open and closed conversations and they can easily go in and participate in live conversations with customers and close them when they are done. Customers love it and Gabe loves it. 


## Solutions
### Features for MVP:
- A customer lands on a site specific to a business where they start a conversation with that business’ client success reps. They give personal info (name, email/phone number), and can login. 
- A customer can see a thread of responses and back and forth with a client success rep, and can re-authenticate to see previous conversations.
- An admin can add or remove “support team” members
- Agents can log in to see pending conversations
+ Agents can add responses to conversations or mark them as closed
- Unauthorised customers that can ask quick questions without conversation tracking. Will still keep track of the convo
 support staff can reassign tickets to different people depending on expertise/knowledge area. There will only be one agent per conversation at any given time.
Support staff 5 star rating with optional message

### Features for future releases:
- Metrics on admin dashboards that show a breakdown of agent performance across KPIs such as average customer rating, vol tickets handled. (Possibly show a leaderboard to agents and gamify?).
- Responses are sent to the end user via email with a link back to the conversation. 
- Responses are sent via SMS with a link to the conversation.
a list of priority emails that marks certain users as highly important.
- Support team receives tickets or updates on existing tickets via slack.
some option to make an intelligent bot then can use these frequently asked questions.
- User’s get feedback when other user is typing

### Features for future future releases:
- Stretchy stretch stretch (if move towards bot idea) https://dialogflow.com/ NLP/Sentiment/Bot Automation
- Stretchiest stretch stretch - chat in multiple languages - https://cloud.google.com/translate/docs/


## Why build this?
### What problem does this application solve?  
1. Businesses are looking for a streamlined workflow for managing and handling support requests:
    1. Agents previously had to work across multiple tools causing inefficiency in their response times
    2. There was no means of tracking tickets meaning some customers queries could have gone on unresolved.
2. Customers are looking for direct lines of conversation with minimal fuss:
    1. The user experience was fragmented, submitting an email, receiving a ticket, and finally getting to support
    2. There was no feel of engaging with a real member of the team and being able to converse naturally back and forth.

### How does your application solve the problem?  
  1.1 All conversations are in one place, as well as the ability to respond to customers.

  1.2 Each ticket is tracked with an ID, a status indication, a history of agents that have worked on it, and a history of all other tickets the customer is associated with.

  2.1 The user experience is bound to a chat window where customers either engage with agents.

  2.2 Live chat gives the customer a direct line of conversation.

## Key Features
### What is the “bread and butter” of your app? What makes your app yours? 

*Discuss as a team how long it will take to implement these features. Can you build it in the first 3 weeks? (Note: It is preferred to drop features and spend more time working on these key features.)*
1. Live chat between agents and customers. 
2. Seamless integration with user’s websites and digital assets via a lightweight JS code snippet.
3. End to end ticket tracking and handling.

**Brainstorming** - how do we find an unique angle and no just build watered-down Intercom?

- Customer support as a service for start-ups, pool of agents wrapped around a chat app that clients can easily add to their websites.
- Specific industry where we can tailor specific needs e.g. taxis (possibly interview members from that industry to determine one or two twist features).
- New-never-before-seen-features: video chats for B2B  support.

Potential challengers and time consumers
- Creating a code snippet for integration with customer sites.
- Using a no-SQL database for the first.
- Using Socket.io.

## Competitive Landscape
### Who are your competitors and how do they solve this problem? List at least three. Link to screenshots or samples features.

Competitors are solving the customer support problem in a similar way (via chat applications and support dashboards) - the points of differentiation are generally around specific features:

**Unite customer queries from all touch points (social, email, brand.coms)**   
Zendesk, Intercom, Kayako   
https://www.zendesk.com/support/

**Utilising conversation data for improved support**   
Zendesk - create company knowledge bases and FAQ pages based on conversation data - https://www.zendesk.com/guide/   
Drift - automate support conversations based on previous data   
LivePerson - creates ticket order based on sentiment analysis of text   
Dialog flow - pulls Google data to create smart chatbots that can be used in customer interactions

**App marketplaces with a suite of plugins and integrations to fit existing tech**   
Zendesk - get chats working across global languages. - https://www.zendesk.com/suite/   
Chatlio - integrates ticket support for teams that already use Slack.

**Cater to different industries and client sizes**   
Zendesk, Intercom -  industry-specific features and pricing structures for different business sizes


### How many types of user accounts will you need for this project?  For each user account type, answer the following:

**Account Type:** App Owner   
**Description:** Owner of the application.   
**Needs:** Access to everything; create admin accounts, manage billing.


**Account Type:** Admin   
**Description:** Customer support team leads.   
**Needs:** Complete overview of ticketing system, ability to assign and reassign tickets to agents, metrics on agent performance, ability to create agent accounts, (Admin has all of the same rights as an Agent and can respond to tickets also as a requirement for smaller teams where admin and agent roles have overlap).


**Account Type:** Agent   
**Description:** Customer support worker.   
**Needs:** Complete overview of ticketing system, respond and engage with tickets, close tickets, reassign a ticket that they’re working on (if expertise elsewhere is  required).


**Account Type:** Customer   
**Description:** End user.   
**Needs:** Timely resolution to their queries.

## Monetization

### Which users would be willing to pay for your app?
Larger businesses with more throughput - one admin and one agent for free, extra cost per agent or admin /month.
.
### What features can you charge for in your app?
Agent performance metrics dashboard on admin accounts, Slack integration

### Is there a possibility of a subscription model? Or a one time purchase?
Monthly subscription for extra admins/agents.






## Features

A new customer finds the Co for the first time and has a quick question to further his research.

### For each feature in your spec answer the following:

**Feature Name:**   
*   ***User access:**   **   
**2-3 User Stories:** As a _____ I want to _______ so that_________   
**What internal APIs will you build to implement this feature?**   
**Are there third party services, APIs, or platforms will you use to implement this feature?**   
**Have you considered using native frameworks?**   
**What are the costs and benefits of using the third party solution?**



## Views
### For each view in your spec answer the following:

**View Name:**   
 Button chat now plugin   
**User access:**    
customers   
**How will the user navigate to the view?**    
The landing page of third party website   
**What elements/animations will you use to create the view?**   
Button with hover effect.   
**Are there third party services, APIs, or platforms will you use to implement this view?**   

**What are the costs and benefits of using the third party solution?**



**View Name:**   
Customer login / problem statement    
**User access:**   
Customer   
**How will the user navigate to the view?**   
Via the button chat now plugin.   
**What elements/animations will you use to create the view?**   
Form to collect user info and problem statement.
Button ask quick question without being a registered user.

Button Saved convo
    When clicked shows 
    Input for email
    Input for password
Button to sign up
Input name required
Button to start chat
   
**Are there third party services, APIs, or platforms will you use to implement this view?**   
APIs
Login (maybe o auth)
Register (maybe o auth)


**What are the costs and benefits of using the third party solution?**



**View Name:**   
Customer chat model   
**User access:**   
Customer   
**How will the user navigate to the view?**   
By joining old chat or making a new chat from ‘Customer login / problem statement’ view.   
**What elements/animations will you use to create the view?**   
Textbox for typing message
Button for closing chat model
Button for sending message
Div for chat bubbles
Img for picture of agent
Headers for Agent name and for agent motto
    
**Are there third party services, APIs, or platforms will you use to implement this view?**   
APIs
Connect to chat
Third party services
Socket.io 
**What are the costs and benefits of using the third party solution?**



**View Name:**   
Employee login   
**User access:**      
**How will the user navigate to the view?**      
**What elements/animations will you use to create the view?**      
**Are there third party services, APIs, or platforms will you use to implement this view?**   
APIs
Login (maybe o auth)
Register (maybe o auth)
**What are the costs and benefits of using the third party solution?**


**View Name:**   
Support team view   
**User access:**   
Agent , admin or super admin   
**How will the user navigate to the view?**   
For Agent
From login 
For Admin
From admin navbar   
**What elements/animations will you use to create the view?**   
Current chat
Textbox for typing message
Button for ending chat
Button for sending message
Div for chat bubbles
Headers for customer name, email and customer question
    Customer name and email link to customer record search
Tickets
    Navbar for active, queued and closed tickets subviews
    Count of tickets
    active, queued and closed subview all have
        A list of cards 
            Each card has the customer’s question and maybe name   
**Are there third party services, APIs, or platforms will you use to implement this view?**   
APIs
Connect to chat
Get queued tickets
Get closed tickets
Get active tickets
Put queued ticket to change ticket state (active, queued or closed)
Third party services
Socket.io 
**What are the costs and benefits of using the third party solution?**



**View Name:**   
Chat log    
**User access:**   
Admin, agent and customer   
**How will the user navigate to the view?**   
Admin and agent 
by clicked on the closed ticket card
Customer 
via link
   
**What elements/animations will you use to create the view?**   
Img for picture of agent
Headers for Agent name, customer name, customer email and customer question
A list of the messages sent in this chat
    Each message has the name of the sender followed by the message.
The date and time of the chat ending. Rating part for customers only
The score of the chat if the user already rated the chat. If the user did not rate the chat ask for the rating.   
**Are there third party services, APIs, or platforms will you use to implement this view?**   
APIs
Get ticket by id
Post ticket score
**What are the costs and benefits of using the third party solution?**



**View Name:**   
Account settings   
**User access:**   
Admin and agent   
**How will the user navigate to the view?**   
Click on settings gear in header   
**What elements/animations will you use to create the view?**   
Input prefilled with email
Input prefilled with phone number
Input for old password required to update anything
Input for new password
Input prefilled with name
Input prefilled with motto
Img with current image
Button to upload a new image
Button to save all updated info
   
**Are there third party services, APIs, or platforms will you use to implement this view?**   
APIs
Get current user info
Put current user info
**What are the costs and benefits of using the third party solution?**


**View Name:**   
Company dashboard    
**User access:**   
Admin and super admin    
**How will the user navigate to the view?**   
Default for super admin login or via navbar   
**What elements/animations will you use to create the view?**   

img for company picture
H for company name
H for company motto
Button or buttons to update customer name and motto

Textbox for Code plugin snippet
Button to copy the code snippet 

List of team members
    Each member has name, email, delete button and a checkbox for if admin. Only super admin can change this checkbox.

Button to add a new team member
   
**Are there third party services, APIs, or platforms will you use to implement this view?**   
APIs
Get company members
Put company member to admin (super admin)
Delete company members
Get company info
Put company info
**What are the costs and benefits of using the third party solution?**


**View Name:**   
Add team member model   
**User access:**   
Admin and super admin   
**How will the user navigate to the view?**   
 By clicking the add new member button   
**What elements/animations will you use to create the view?**   
Input for email
Button for submit    
**Are there third party services, APIs, or platforms will you use to implement this view?**   
**What are the costs and benefits of using the third party solution?**


**View Name:**   
Payment info view   
**User access:**   
Super admin   
**How will the user navigate to the view?**   
From clicking on navbar   
**What elements/animations will you use to create the view?**   
List of different membership plans
Currently selected membership plan
Button to update membership plan
List of payment methods (paypal, credit card ect)
Currently selected payment method
Button to update payment method
   
**Are there third party services, APIs, or platforms will you use to implement this view?**   
**What are the costs and benefits of using the third party solution?**


# Architectural Recommendations
## Front End
**What technology solution will you use for your front-end?**   
**What problems does this solution solve for this specific project?**   
**What are the drawbacks of using this solution over alternatives?**   
React
Do we want to use CRA?
YES
redux


## Design Framework
**What library or framework will you be using for styling and presentation?** (We highly recommend using a third-party component library - we will help pay for premium themes)   
**What problems does this solution solve for this specific project?**   
**What are the drawbacks of using this solution over alternatives?**


## Back End
**What technology solution will you use for your back-end?**   
**What problems does this solution solve for this specific project?**   
**What are the drawbacks of using this solution over alternatives?**   
Node
express
Socket io over just websockets


## Deployment
**What technology solution will you use to deploy your front-end and back-end?**  

**What problems does this solution solve for this specific project?**

**What are the drawbacks of using this solution over alternatives?**

Heroku/Zeit-Now/Netlify/Firebase
Cost estimate when running at scale


## Database
**What technology solution will you use for your database?**

One of the main considerations for picking a database was to either choice a SQL or NOSQL database. Since our app involves realtime chat the number one consideration data wise for our app is read and write speed. Another key aspect that was decided  on was scalability. Referring to the below table and thinking about the mentioned requirements for the database  it was decided that a NOSQL technology would be selected. 

Carla Andres table comparing relational to NOSQL databases
From reviewing a number of different NOSQL databases mongoDB was selected for these reasons :
- Ease of scaling via automatic scaling ( Sharding)
- High performance 
- Secure from SQL injection
- Supported by a large community (lots of resources)

**What problems does this solution solve for this specific project?**
- Quickly deliver messages to users.
    Since mongoDB has a fast read and write speed it should allow for live messages to get delivered to the users quickly. This is partly because  MongoDB does INSERT and UPDATE  Asynchronous (eventual consistency).
- Allow for rapid scaleility 
    MongoDB offers auto sharding which allows for the database to grow horizontally over many servers rather then growing vertically. This is advantageous because horizontal growth is cheaper then vertical growth

**What are the drawbacks of using this solution over alternatives?**
- MongoDB is not as reliable as a traditional SQL DB
    MongoDB inserts and updates data asynchronously. This means that there is no return value for a successful insert or update. This allows for a faster insert or update but results in no confirmation that the operation was successful. Since speed is more important than reliability this is an acceptable trade off.
 
- No capabilities of a  relational database.This means no joins. 
    Since a NOSQL DB is being used it will have to be designed in a way that makes sense for the technology. In some cases it could be seen as a positive that there are no joins. 

## Model
**What data do you need?**

User information [username, name, email etc]
Employee data [employeeID, username, name email etc]
Admin data / can be a selected employee
Chat logs 

**Where will you get the data?**

On our database which we have chosen at the top 

**Will your data be stored locally on your front-ends (Mobile, FE Web)?**

If we store it locally we will have a lot of data to handle but if we use database of our choice then import it when needed i guess
**How is your data related?**

**What models do you need to represent your data fully in the database in a manner that is logical and consistent? For each model, show properties and initializers.**


# APIs - Internal and Third Party Services
## Feature List
**For each feature identified above, add the following information.**   
(Every feature should be listed and considered)


### Feature Name:
**What internal APIs will you build to implement this feature?**

**Are there third party services, APIs, or platforms will you use to implement this feature?**

**What are the costs and benefits of using the third party solution?**




# Outline and Weekly Plan
## Weekly Plan

**Look in Training Kit to find the weekly objectives. For each week create a plan for what will be implemented:**   
(Map out every week)


### Week X:
**What are the key goals you will accomplish?**

**What features or services will be completed?**


## Summary
Use the information above to fill out the following table:

|Name: | Web chat app |
|:---|:---|
|**App description:**| Web chat app is an application that solves ... by ... |
| **Front End:** | this | 
| **Back End:** | that |
| **Database:**  | that |
| **List of APIs:** | 
| - one |
|  - two |
| **List of Additional Services:**|
|  - one |
|  - two |



# References 
1. CARLA ANDRES (2017, April), NoSQL Databases: The Definitive Guide. Retrieved on April 23 2019, from https://blog.pandorafms.org/nosql-databases-the-definitive-guide/



 


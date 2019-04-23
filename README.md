# webchat-documentation

Repo for projects documentation

## Architectural Recommendations

### Front End

What technology solution will you use for your front-end?
What problems does this solution solve for this specific project?
What are the drawbacks of using this solution over alternatives?

React with Redux for global state management.

This solution will allow us to render UI components dynamically with state changes, whilst also making asynchronous calls to the backend. React will give us flexibility to build a highly modular and, therefore reusable and testable, set of components. In this particular project, the solution allows us to display all of our linked views across the ticket support display, user acount details, and customer chat modal, whilst (1) readily updating the recorded conversation, the status of tickets, and their assignees, and (2) handling user authentication requests and their associated views.

React gives us complete flexibility over which other libraries we may want to integrate within our application, when compared with framework solutions such as Angular and Vue. As a project that may in future look to deliver a native mobile solution that smaller customer service teams can use on the go (as in the case of webchat support competitors), React also offers the ability to re-use the bulk of our code base in a React Native setting. A potential drawback of using React over alternative options is that Vue is slightly more lightweight, requiring less memory and generally running faster when the same application is built on both technologies. Although it is possible to write React applications in Typescript, Angular's coupling with the Typescript language makes for a solution that most effectively covers type-checking and reduces room for such type errors that can occur in dynamically-typed Javascript. This downside can be somewhat limited by introducing prop-type checks across our React application.

### Database

(refer to stand alone tech docs for diagrams)
What technology solution will you use for your database?

One of the main considerations for picking a database was to either choice a SQL or NOSQL database. Since our app involves real-time chat the number one consideration data wise for our app is read and write speed. Another key aspect that was decided on was scalability. Referring to the below table and thinking about the mentioned requirements for the database it was decided that a NOSQL technology would be selected.

![table comparing relational to NOSQL databases](images/relationalvsNOSQL.PNG)
Carla Andres table comparing relational to NOSQL databases

From reviewing a number of different NOSQL databases mongoDB was selected for these reasons :

- Ease of scaling via automatic scaling ( Sharding)
- High performance
- Secure from SQL injection
- Supported by a large community (lots of resources)

What problems does this solution solve for this specific project?

- Quickly deliver messages to users.
  Since mongoDB has a fast read and write speed it should allow for live messages to get delivered to the users quickly. This is partly because MongoDB does INSERT and UPDATE Asynchronous (eventual consistency).
- Allow for rapid scalability
  MongoDB offers auto sharding which allows for the database to grow horizontally over many servers rather then growing vertically. This is advantageous because horizontal growth is cheaper then vertical growth

What are the drawbacks of using this solution over alternatives?

- MongoDB is not as reliable as a traditional SQL DB
  MongoDB inserts and updates data asynchronously. This means that there is no return value for a successful insert or update. This allows for a faster insert or update but results in no confirmation that the operation was successful. Since speed is more important than reliability this is an acceptable trade off.
- No capabilities of a relational database.This means no joins.
  Since a NOSQL DB is being used it will have to be designed in a way that makes sense for the technology. In some cases it could be seen as a positive that there are no joins.

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
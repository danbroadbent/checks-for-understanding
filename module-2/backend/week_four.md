## Week Four Recap

### Instructions
Fork this repository. Answer the questions to the best of your ability.

Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week.

Note: When you're done, submit a PR with a reflection in the comments about how this exercise went for you.

### Questions

* What is a cookie?<br />
  A cookie is a file saved on a users browser that maintains information between http requests.
* What’s the difference between a session and a cookie?<br />
  A session is a cookie that is only valid for one user session.  Used to keep track of a logged in user.
* What’s a flash and when do you want to use flashes?<br />
  A flash sends a one time notification to a user that expires instantly.  Good for telling a user something that they created or editied was successfully saved.
* Why do people say “HTTP is stateless”?<br />
  HTTP doesn't retain information along requests, each request is independent, so it can't maintain a state.
* What’s authentication? Explain.<br />
  Authentication is verifying a user is who they say they are.  Authentication is used to link a person to a user account, the person will create an account with a username and password, and this will be used to verify they are who they say they are.
* What’s the difference between authentication and authorization?<br />
  Authorization gives different access to different pages depending on usertype.  Once a user has authenticated, then authorization will determine what pages they are allowed to view.
* What’s a before filter?<br />
  A before filter is a method that runs before any other code, it is used to make sure a user is authorized before they hit the route they requested.
* How do we keep track of a user once they’ve logged in?<br />
  Sessions are used to keep track of a logged in user.
* When do you want to namespace a resource? When do you want to nest a resource? What's the differences between those two approaches?<br />
  A namespaced resource creates a nested looking path, however the namespace is not a resource.  In a nested resource, there are two resources where one belongs to the other and can't exist without the other.
* At a high level, what tools can you use to implement authorization? How would you use them?<br />
  you can use a current user helper method to keep track of the current user, you can use an enum to keep track of the different roles of users, you can use before filters to keep certain user types out of certain pages, you can also filter content in views depending on a user's role
* What's an enum, and what advantages does it offer? What data type needs to be in your database to use an enum? Where do you declare an enum?<br />
  an enum is an active record method that helps you assign and keep track of different user roles for authorization.  It comes with custom methods.  It is an integer in the database.  It is declared in the user class.
* What are some strategies you can use to keep your views DRY?<br />
  partials, helper methods, before actions

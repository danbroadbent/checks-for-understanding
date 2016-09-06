## Week Three Recap

### Instructions
Fork this repository. Answer the questions to the best of your ability.

Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week.

Note: When you're done, submit a PR with a reflection in the comments about how this exercise went for you.

### Questions

1. What are the 3 main features in an ERD?<br />
Objects, relationships, and cardinality
2. Create an ERD for the following database: Restaurants, Customers, Items, Ingredients, Beverages, Orders, Vendors.
3. What is the entry at the command line to create a new rails app?<br />
rails new name_of_app
4. What do Models generally inherit from in rails?<br />
Active Record
5. What do Controllers generally inherit from in a rails project?<br />
Application Controller
6. How would I create a route if I wanted to see a specific horse in my routes fitle assuming I'm sticking to standard conventions and that I didn't want other CRUD functionality?<br />
resources :horses, only: [:show]
7. What rake task is useful when looking at routes, and what information does it give you?<br />
rake routes gives you all your availble routes, the prefix, the http verb, path information, controller action.
8. What is an example of a route helper? When would you use them?<br />

9. What's the difference between what `_url` and `_path` return when combined with a routes prefix?<br />
_url will give a path that includes the domain name, and _path gives you a path relative to the project root.
10. What are strong params and why are the necessary?<br />
Strong params are for defining what parameters can be passed through your forms, it helps protect from people hacking your site.
11. What role does `form_for` play in helping us create our forms?<br />
It allows us to use the attributes of our models to create html forms.
12. How does `form_for` know where to submit the user's input? <br />
It is linked to a model, so it is associtated with that class's active record.
13. Create a form using a `form_for` helper to create a new `Horse`. <br />
`` <%= form_for(@horse) do |f| %><br />
<%= f.label :name %><br />
<%= f.text_area :name %><br />
<%= f.submit %><br />
<% end %> ``
14. Why do we want to validate our models?<br />
We want our data coming into our database to be in the correct format.  For example if we want all our horses to have a name, we can validate that it does before it can be saved into the database.

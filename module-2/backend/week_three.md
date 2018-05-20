
1. What is the entry at the command line to create a new rails app?

* rails new (appname)

2. What do Models generally inherit from in rails?

* They generally inherit from ApplicationRecord.

3. What do Controllers generally inherit from in a rails project?

* They generally inherit from ApplicationController.

4. How would I create a route if I wanted to see a specific horse in my routes file assuming I'm sticking to standard conventions and that I didn't want other CRUD functionality?

* resources :horses, only[:show]

5. What rake task is useful when looking at routes, and what information does it give you?

* rake routes shows all the lists of paths we have available and also helps us to
  determine when sending instance variable to views.

6. What is an example of a route helper? When would you use them?

* horses_path is an example to see horses index. I would use those in testing, for links and
  whenever i have to redirect.

7. What's the difference between what `_url` and `_path` return when combined with a routes prefix?

* _url gives us full url path including host, protocols etc. _path gives us info about just the paths.
8. What are strong params and why are they necessary?

* strong params part of the params(key value pair) that we need by defining in private
* to avoid unnessessory things reach our model we use strong params(security reason.)

9. What role does `form_for` play in helping us create our forms?

* form-for helps us to create a post request without us telling it to do post
  requests.

10. How does `form_for` know where to submit the user's input?

* based on the instance variable we pass in in the form it determines where to send
  the post requests.

11. Create a form using a `form_for` helper to create a new `Horse`.

* <%=form_for @horse do |f| %>
  <%=f.label :name %>
  <%=f.text_field :name %>
  <%end%>

12. Why do we want to validate our models?

* we want to make sure only valid data is saved in our data.

13. What are the steps of the DNS lookup?

*


### Review Questions
14. How would you call the method `prance` from within the method `move` on a `Horse` instance?

def move
  prance
end

15. Given the following hash:

furniture = {table: {height: 3, color: "red"}, purchased: true}

What is the different between how you would return true vs returning 3?  

* we have to call two keys to get 3 but to get true, just have to call the key purchased.we have nested hash here.

16. What is inheritance?

* Inheritance is process of making a class that resembles the characteristics
of a class inheriting from . helps us to utilize methods that already exists in superclass.

### Self Assessment:

* I was able to answer every question without relying on outside resources

* I feel comfortable with the content presented this week

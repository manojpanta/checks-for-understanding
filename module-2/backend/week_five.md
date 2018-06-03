### Week 5 Questions

Re-pull from this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week (which is a TON!).

Note: When you're done, submit a PR.

### Week 5 Questions
1. How do we make flash messages display on a page?

  * flash[:notice] = 'something' before redirecting

  * and in application.html.erb

  * <% flash.each do |name, msg| %>
    <%= content_tag :div, msg, class: name %>
  * <% end %>

2. Where is cart information/temporary information usually stored?

  * cart information usually stored in session hash.

3. What might be some reasons not to store a cart in our database? Are there any reasons why we would want  to      persist that information?

   * we dont want to store all those added datas if user decides not to checkout, which causes unnecessary usage of storage

4. What is the purpose of the asset pipeline?

  * helps fixing production environment problems.

5. Why do we precompile our assets?

  * we usually precompile our assets so our html file doesn't have to talk to css files multiple times.

6. What do each of the following tags do?


```ruby
<%= stylesheet_link_tag "application" %>

 * will include the stylesheet named application.css

<%= javascript_include_tag "application" %>

* includes some javascript file called application

<%= image_tag "rails.png" %>

* image_tag will automatically add assets at start of the path

```

7. What are some of the elements of a great read me? What are some of the benefits of taking the time to update a readme for our project?

 * Readme can be great for users to know how does the app work.

8. What are the top four accessibility issues that we as developers should be aware of?


9. `before_save` is an example of a what? Where in our Rails application would we find a `before_save`?

  * before save is an example of callbacks. we  can use callbacks in models.

10. Given the following object, how would we create a scope for all users who are active?

 * before_action :current_active? (we have to create a methos like this to check if they are active.)

```ruby
User.create(name: "Happy", active: true)
```

11. What is the difference between a scope and a class method

### Review Questions:  
12. Given the following hash:  

```ruby
{cart: {"17" => 4, "204" => 52, "29" => 22}}
```

  12a. How would you add item with id of 48 with a quantity of 4?  
    * given[:cart]['48'] = 4
  12b. How would you increase the quantity of item 29?  
    * given[:cart]['29'] += 1
  12c. How would you find out how many items your user is thinking about purchasing?
    * given[:cart].values.sum

13. What is polymorphism? How does it relate to duck-typing? What are two ways you use this in everyday Rails applications?  
14. How would you clean the string "(630) 854-5483" to "630.854.5483"?  


### Self Assessment:
* I was able to answer most questions independently, but utilized outside resources for a few

Choose One:
* I feel confident about the content presented this week
* i feel pretty good abut the lessons we had this week but i got stuck on some of these questions.

common verbs in http
      * get, post

      get verb is used to get info from the server as oppose to post which provides
      info to the server.

      * put

      put verb is used to  update a content

      * delete

      to delete

      * patch
      patch is used to update or replace  content

what is sinatra?
 * sinatra is a software web application library


what is MVC?

MVC stands for Modle views and contriller. I think HTTP works with the principle
of mvc.


we have to follow the convention because activerecord and sinatra works thst way only
such as: naming things plural or singular in many cases matters.


instance variables from controllers are available in erb files.


this is how we pass instance variable to erb files
get '/horses' do
@count = 1
  erb :index
end


8. In the same code block, how would I pass a local variable `name` with a value of `Mr. Ed` to the view?


ERB is being use to translate ruby into html.
we need development and test database to make sure we do not mess up our
datas.


CRUD is list of operations we can perform on a resource.
create  read update and delete.

HTTP stands for hypertext transfer protocol.


following are the two ways to interpolate ruby in an ERB file.
<%= something %>
<%end%>

<%something%>
<%end%>


ORM is Object relational mapper
Activerecord is the most commonly used orm in ruby.


seven verb and paths for application with restaurants.


1.get "/" do
end

takes us to homepage

2. get "/menu" do
end

takes us to menu of that restaurant.

3. post '/new-account' do
end
lets us make a new account

4. get '/customers' do
end
shows us the customer lists.

5. delete '/customers' do
end

once we click delete button for a customer profile then server deletes the account
through this path.

6. put '/customers/:id' do
end

we can modify profile of a customer through this path.



what is migration?

migration migrates data to the database.
when we create a migration , it modifies the database.

Model asks database the info asked by the controller.

# new is to make new instance of a class
# create is active record method to make new instance of a model.

this is how we create instance of Film using csv file.
films = Csv.open(.......)
films.each do |film|

Film.create(id: film[id]
            title: film[title]
            description: film[description])

end



How would I add 'granola bar' to things you should have when hiking?
23. What are the 4 Principles of OOP? Give a one sentence explanation of each.
activities = {
  hiking: {cost: $0, supplies: ['hiking shoes', 'water', 'compass']},
  karaoke: {cost: $10, supplies: ['courage', 'microphone'],
  brunch: {cost: $35, supplies: ['mimosa flutes'],
  antiquing: {cost: $200, supplies: ['list of antique stores']
}


answer : activities[:hiking][:supplies] << 'granola bar'




### Self Assessment:
* I was able to answer most questions independently, but utilized outside resources for a few

Choose One:
* I feel comfortable with the content presented this week



1. At a high level, what is ActiveRecord? What does it do/allow you to do?
  Active record is a library that helps us with database relationship  using SQL
  but invery simple way.

2. Assume you have the following model:


class Team << ActiveRecord::Base
end

What are some methods you can call on `Team`? If these methods aren't defined in the class, how do you have access to them?

  we can call Team.all to find all the elements for Team table
  We can call Team.create(attributes) to create a Team object.
**activerecord has all those methods, we can call them on Team as Team is inherited
from Activerecord: :Base

3. Assume that in your database, a team has the following attributes: "id", "name", owner_id". How would you find the name of a team with an id of 4? Assuming your class only included the code from question 2, how could you find the owner of the same team?

  team = Team.find(:id)
  team.name

  owner = Owner.find(team.owner_id)

4. Assume that you added a line to your `Team` class as follows:

class Team << ActiveRecord::Base
  belongs_to :owner
end

Now how would you find the owner of the team with an id of 4?
  team = Team.find(:id)
  owner = team.owner

5. In a database that's holding students and teachers, what will be the relationship between students and teachers? Draw the schema diagram.


6. Define foreign key, primary key, and schema.
  *primary key is the id created by database
  *forign_key is a column of ids in a table which is primary key in other table
  *schema is a structure of a table in a database.
7. Describe the relationship between a foreign key on one table and a primary key on another table.
  * we have access to the elements on second table using forign key from first table  if that foreign key is
    primary key on second table.
8. What are the parts of an HTTP response?
  *Head(contains details about the request, info about whether that request was valid , status code methods etc. )
  *body(response user sees)


### Optional Questions

1. Name your five favorite ActiveRecord methods (i.e. methods your models inherit from ActiveRecord) and describe what they do.
  *all(we can see all the elements in a table)
  *create(we can directly add elements to the table )
  *update (we can update elements in a table with out writing all the sql queries)
  *destroy(deletes elements from a table)
  *joins(joins two tables together)
2. Name your three favorite ActiveRecord rake tasks and describe what they do.
  *rake db:create (creates database for us)
  *rake db:migrate (migrates the table structure to the database and creates schema.)
3. What two columns does t.timestamps null: false create in our database?
  *created_at
  *updated_at
4. In a database that's holding schools and teachers, what will be the relationship between schools and teachers?
  schoos have many teachers
  teacher belong to school.
5. In the same database, what will you need to do to create this relationship (draw a schema diagram)?
6. Give an example of when you might want to store information besides ids on a join table.
  *say merchants have many items and item belong to merchant, if we want to find
  average item price for a merchant then i want to join tables with avg_price, that
  way i dont have to go back to database everytime i want to find avg item price
  for a merchant.
7. Describe and diagram the relationship between patients and doctors.
8. Describe and diagram the relationship between museums and original_paintings.
9. What could you see in your code that would make you think you might want to create a partial?
  *if we are using the same thing in various places i want to make a partial and
  call that file whenever i need. i can compare that with module.

### Self Assessment:
I am little bit confused about the diagram thing above .everything else was
fine.
* I was able to answer most questions independently, but utilized outside resources for a few

Choose One:
* I feel confident about the content presented this week
 but i feel like i have to work on joining tables a little bit more.

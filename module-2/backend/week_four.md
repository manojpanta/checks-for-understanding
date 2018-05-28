## Week Four Recap

### Instructions
Fork or re-pull this repository. Answer the questions to the best of your ability.

Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week.

Note: When you're done, submit a PR with a reflection in the comments about how this exercise went for you.

### Week 4 Questions

1. What is a cookie?

* cookies are files that contains data about particular client and website

2. What’s the difference between a session and a cookie?

* cookies are stored in user's computer but sessions are stored in server

3. What’s a flash and when do you want to use flashes?

* flash is message that appears on page upon some actions. we want to use flash
  to let the user know they have done some action.

4. Why do people say “HTTP is stateless”?

* Http is stateless because it doesnt know previous request datas.(or doesnt
  remember previous datas of an user)

5. What’s authentication? Explain.

* Authentication is verifying user if they are valid user.

6. What’s the difference between authentication and authorization?

* Authentication lets you in to your website but authorization gives you options
  based on your authentication details.

7. What’s a before filter?

* before filter makes decision whether should a user be allowed to some actions.

8. How do we keep track of a user once they’ve logged in?

* using session

9. When do you want to namespace a resource? When do you want to nest a resource? What's the differences between those two approaches?

* Namespace is typically used for authorization.
* Nesting is used if some thing is dependent on something.

10. At a high level, what tools can you use to implement authorization? How would you use them?

* enum can be used for authorization.

11. What's an enum, and what advantages does it offer? What data type needs to be in your database to use an enum? Where do you declare an enum?

* enum is a tool for authorization process.
* it uses hash.
* we declare enum in model level

12. What are some strategies you can use to keep your views DRY?

* by not using activerecord calls from views
* by not using conditionals that actually calls our database.


### Reviews Questions
13. Given the following array of hashes, how would I print an alphabetical list of holidays?
```ruby
[
 {holiday: {name: "St Patrick's Day", supplies: ["Corned Beef and Cabbage"]},
 {holiday: {name: "Halloween", supplies: ["Candy", "Costume"]},
 {holiday: {name: "Hanukkah", supplies: ["Menorah"]}
]
```
given.map do |g|
  g.values[0]
end.sort


*   
14. How would you clean incoming data to ensure "$300" or "300.00" is stored as 300?


### Self Assessment:
* I was able to answer most questions independently, but utilized outside resources for a few

Choose One:
* I feel confident about the content presented this week
(I'm still practicing git rebase.)

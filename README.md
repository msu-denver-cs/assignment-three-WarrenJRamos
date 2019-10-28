# README
What did I do?
First of all, I reread the Authentication PowerPoint, and made sure to follow all the instructions listed in
the PowerPoint to add authentication functionality to my web application using the Devise gem. The only action I did 
differently from the PowerPoint was that I added the before_action hook to my application_controller.rb file because 
I noticed that all the controllers derived from the application_controller. Instead of changing the before_action to 
each controller, I added it to only one file which was more concise.
After I finished authentication using the Devise gem, I added a simple navbar table. It worked, but I wanted to make the
navbar look pretty, so I ended up using Bootstrap which one of my peers recommended me to use. I followed the
Bootstrap documentation and other tutorials online to add a Bootstrap navbar to my application. However, I ran into some 
errors when I added the Bootstrap gem to my Gemfile. The error had something to do with the Devise gem and an image I 
used in my cars index.html. 
After trying to resolve all the errors, I was still unable to fix it within 4 hours, so I restarted the whole project. This time, I started 
with the Bootstrap navbar, and then I added authentication using Devise, and everything just worked (no more errors). To add the navbar
to all my pages, I put the navbar in the application.html.erb in the layouts folder so that each page would render the navbar.
In the end, I was successfully able to accomplish all of the requirements for this project: the completion of authentication 
and a navbar.
Furthermore, I added a logout option to all of my index pages so the user can log out. I then made my root page the cars index 
page by adding "root to: "cars#index" in the routes.rb.

What commands did I issue? 
* bundle install
* rails generate devise:install
* rails generate devise User
* rails db:migrate
* rails routes 

What did you learn?
I learned about authentication, how to create a simple navbar, and how to create a navbar through Bootstrap. I actually did
not know what a navbar was until this assignment, and I discovered how useful it is to have a navbar on a web application so 
that users can simply click on something to get to another page.
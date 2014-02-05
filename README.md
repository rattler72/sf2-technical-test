# EA Symfony2 Technical Test

### Task

* The task is implement a website that allows the user to login to search the Github repoistories.
* You have 4 hours to complete the test.
* Please finish all the items outlined in the Requirements section first, then try to tackle items in the Nice to Haves section if you have time.
* If you cannot finish the test, please explain why as we are reasonable and realize people have time constraints.

### Setup

* You can find the design under the design folder
* You would need php5.5, Symfony 2 and a web server to run the application
* To see if the app running, http://localhost/app_dev.php/ or http://localhost/app_dev.php/demo/hello/Fabien

### Requirements

* You are free to use 3rd party authentication bundle or build your own bundle
* The login form should have server side validation
* All pages should be gated by the login page if the user is not login.
* You are free to use any http client to call out to Github's API
* Have a search field that allows searching for a GitHub user's repositories. See http://developer.github.com/v3/repos/#list-user-repositories for more info. Call the following API (where USER_NAME is the value typed into the search field):
```
https://api.github.com/users/USER_NAME/repos
```
* Once the search is clicked, the results should show a list of that user's public repositories with each item in a "name/number of watchers" format.
* The results should be in json format for the view to consume
* It's not a requirement to style the pages
* We expect to have unit test code coverage of your code

### Nice to Haves

* When a result is clicked, display an alert box with the repository's ID and the created_at time.
* Use AngularJS to display the repositories results
* Extended functionalities where you see fit.

### Deliverables

* Please fork this project on GitHub and add your code to the forked project.
* Update the README file to include the time you spent and anything else you wish to convey.
* Send the link to your forked GitHub project to your recruiter.

*Good luck!**

#My Notes - Stacey Friesen

##Overview
I spent about 3.5 hrs on this task. This is my first time actually developing with Symfony 2. As I mentioned in my phone interview, I have been developing most recently with Laravel 4, which is based off of the symfony components. Unfortunately, I did not finish the task as I had hoped. I was learning the nuances of the framework and in particular got hung up on the authentication and routing for the app. 

##Setup
When I received the task, I spent an hour setting up my environment. I had to upgrade from PHP 5.4 to 5.5... and had a few bumps upgrading that and composer. After everything was set up, I downloaded the framework and used composer to install the libraries. 

##What I did not complete
Since this was my first time using the framework and given the time constraints, I started by using the demo project to build the authentication functionality. I spent some time learning the conventions of both authentication and routing. As it went... I needed more time for this to fully understand. However I feel, this probably wouldn't take long for me to learn. 

##What I did complete
After struggling a little with the authentication and routing, I jumped into the Github API. Using Guzzle, I was able to create a simple user search. I stopped with about 30 mins to go.

##Where to test?
* http://localhost/app_dev.php/ - Will give you the modified home page.
* http://localhost/app_dev.php/github/login - Is the login page using the demo credentials user / userpass
* http://localhost/app_dev.php/github/browser - This is the github search page. (I tried to secure this page, but removed it after having some trouble with authentication)

##Final Thoughts
I wish this had panned out better for me. I think I could work well with this framework and feel I could get up to speed in a short amount of time (few days...). I hope you consider my effort here and I'd love to prove to you guys that I'm the right fit for the job. Cheers!
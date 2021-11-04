# remoteRailsAPI
Here is a guide on the steps that I took to launch a REST API in Rails! This can be deployed on VPS powered by Linux (I used Ubuntu) to create a secure backend data service that can be accessed anywhere around the world from any front-end application.


Step 1
--------

Determine your goal. 

For an example, I want to be able to be able to view, create, update, and delete several books. Information these items to include would be title, auther, year published, and rating(1 - 5). 

Step 2
--------

Make a plan.

This Ruby on Rails REST API will be performing requests using the methods GET, POST, PUT, and DELETE and the request bodies will be formatted in JSON. For data storage, the API will be linked to a local MySQL database installed on the LInux server. For a front-end, we will be using old fashion HTML, CSS, and JavaScript for this example. You may choose any front-end that you would like to make requests to the API as it is universal.

Step 3
---------

Implementation.

This is a guide that explains everything, including making the API public. If you wish, you may skip these steps and only make this local to test it.

First, you will subscribe to a VPS hosting service. There are many out there. The one I chose to use is http://IONOS.com because it is very affordable. ($5 a month) This is set up with an Ubuntu installation and you get your very own Public IP address.

Next, you will want to make the instance secure. There are plenty of guides on how to do this. One major step that should be taken is to create a new user under root and grant sudo priveleges. Permit Root Login should also be set to off. Here is a quick guide. https://implex.io/posts/ubuntu-20-04-setup/ .

Now that we have the installation secured, we can install Ruby on Rails. Here is a guide to do that. It will be doen using RVM. https://www.howtoforge.com/tutorial/how-to-install-ruby-on-rails-on-ubuntu-1804-lts/ .

Another thing we must do is install MySQL. Here is a guide for doing this. https://www.digitalocean.com/community/tutorials/how-to-install-mysql-on-ubuntu-20-04 . follow the guide to either set a password on the root account or create a new account and password that has the appropriate permissions. Now 'create database bookApp;'.

The next thing that we must do is to install the MySQL gem. Enter "gem install mysql2" inside SSH. You will most likely encounter an error. It will say "libmysql-dev is missing" or an error similar to that. I'm not sure off the top of my head what it was, but type the error in Google and a fix should come up in Stack Overflow.com . Perform the commands that are mentioned to install the required libraries. After those are installed, run "gem install mysql2" again. This time it should be successful.




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

First, you will subscribe to a VPS hosting service. There are many out there. The one I chose to use is IONOS.com because it is very affordable. ($5 a month) This is set up with an Ubuntu installation and you get your very own Public IP address.

Next, you will want to make the instance secure. There are plenty of guides on how to do this. One main 

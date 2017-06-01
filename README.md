# Mean Stack CRUD using Angular Grid and Trix Editor - Visual Studio Node.js Project

Basic MEAN UI - Angular Grid allows adding, editing and removing records from a Mongo DB. Feedback is provided by pop up 'Toast' notifications.



## Project Description




My first Mean app - I wanted to try the basics of CRUD operations on Mongo DB using a Restful API. I also wanted to use Mongoose which seems to be a good and simple ORM for Mongo.
For the UI, I had a look around and there is a lot of good UI angular components available, so I had a go with the Angular UI Grid, the Angular Trix rich text control for an extended HTML style editor
and the NG Toast notifications control. Bootstrap is here as well to make things look nicer.

I'm using Visual studio as I'm a .Net developer, but you can just as well use Express / npm only - just rip all the files out to your own structure and leave out the VS project and solution files.
 
The app just displays a single page with a grid as the main UI. From the grid you can add, edit and remove records. The editor is in a modal window and includes an HTML editor for the 'Template' field 
which stores HTML. Feedback is displayed to the user via toast pop ups.



## Project Set Up

This repositry is setup using MS visual Studio 2013 - you will likely need the 'Node.js' project templates for visual studio - you can check if it's there by starting a new project, 
selecting 'javascript projects' and seeing if node.js is available.

Get the tools here:

https://www.visualstudio.com/vs/node-js/


Once you've grabbed the code, you'll probably need to install the npm packages - you can either do that manually in solution explorer (one by one), or go to the root of the solution and enter  in 
a command window:

npm install



Next, ensure that app.js is set as the startup file.

Then, have a look at the config.js file - here you can set host, DB, port etc. You can leave the defaults if you are running it locally.


## Project Run

You'll need your instance of Mongo DB started by running command prompts:

Mongo Start:

"C:\Program Files\MongoDB\Server\3.4\bin\mongod.exe"

Mongo Connect:

"C:\Program Files\MongoDB\Server\3.4\bin\mongo.exe"

(Change the above paths to your installation - this is just the default for 3.4).


Hit the 'play' button in VS and the project should get running. If you've set a start up URL on the project it should go straight in, otherwise just open a browser and 
go to the URL we have configured in config.js - default is http://localhost:3000/.

You should see the empty grid - now add a record or two, edit them and remove to test it all.




## Components used


Node.js
Mongo DB
Express
Angular

npm - Package manager 
Morgan - Standard Logging to console - https://github.com/expressjs/morgan
Mongoose - Provides an ORM for Mongo - http://mongoosejs.com/
Angular UI Grid - Excellent grid for Angular - http://ui-grid.info/
Angular Trix - Rich text edit control for Angular - http://sachinchoolur.github.io/angular-trix/
NG Toast - Pop up notifications for Angular - http://tamerayd.in/ngToast/




## Tutorials etc I've used to get this together

http://embed.plnkr.co/WLuKSRX5GqH4rXFhGuyo/ (Grid)
https://www.djamware.com/post/58cf4e1c80aca72df8d1cf7e/tutorial-building-crud-app-from-scratch-using-mean-stack-angular-2 (Crud)
http://plnkr.co/edit/hSzwlzUmRQoUtZJke2C4?p=preview (Trix)


# _Eau Claire's Stylist Log_

#### By _Erin Timlin_

#### _A C# web application using MySQL that a user can add a stylist for a hair salon, and add clients to each stylist. This application can be updated for any business to track employees and their clients._

## Technologies Used

* _.Net 6_
* _ASP.NET Core MVC 6_
* _MySQL Workbench_
* _C# 10_


## Description

### Eau Claire's Salon
_This is a MVC web application to help Eau Claire manage her employees (stylists) and their clients. Claire will be able to add a list of stylists working at the salon, and for each stylist, add clients who see that stylist. The stylists have specific specialties, so each client can only see (belong to) a single stylist._

### User Stories
_As the salon owner, I need to be able to see a list of all stylists._
_As the salon owner, I need to be able to select a stylist, see their details, and see a list of all clients that belong to that stylist._
_As the salon owner, I need to add new stylists to our system when they are hired._
_As the salon owner, I need to be able to add new clients to a specific stylist. I should not be able to add a client if no stylists have been added._

## Setup/Installation Requirements

* _Clone this repo_
* _Open the terminal and navigate to this project's production directory called "HairSalon.Solution"_
* _Within the production directory "HairSalon", create a new file called appsettings.json._
* _Within appsettings.json, input the following code:_
<pre><code>"ConnectionStrings": { "DefaultConnection": "Server=localhost;Port=3306;database=erin_timlin;uid=[YOUR-USERNAME-HERE];pwd=[YOUR-PASSWORD-HERE];" }</code></pre>
<strong>Please note! Make sure to enter your username for MySQLWorkbench in [YOUR-USERNAME-HERE] and password for MySQLWorkbench in [YOUR-PASSWORD-HERE], making sure to remove the brackets!</strong>

# Importing The Database

* Open MySQLWorkBench
* In the Navigator > Administration window, select Data Import/Restore
* In Import Options, select Import from Self-Contained File
* Look for the directory called HairSalon.Solution and pick the file called erin_timlin.sql
* Under Default Scheme to be Imported To, select the New button
* Enter the name of the database: erin_timlin and click OK
* Navigate to the tab called Import Progress and click Start Import at the bottom right corner of the window
* After you are finished with the above steps, reopen the Navigator > Schemas tab. Right click and select Refresh All. The database will appear.
* Navigate back to VS Code, and within the production directory "HairSalon", run <pre><code>$dotnet watch run</code></pre> in the command line to start the project in development mode with a watcher.
* Open the browser to https://localhost:5001


## Known Bugs

* _Editing a stylist adds new stylist_
* _Deleting a stylist does not work_

## License

_Reach out with any questions or concerns and please feel free to make any contributions!_

[MIT](license.txt) (c) _2023_ _Erin Timlin_
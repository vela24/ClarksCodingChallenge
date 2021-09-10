# ClarksCodingChallenge

1.	Provide a simple html page in which a user can enter the following. The page merely needs to be functional and does not need to be styled in any way.
a.	The Home page is connects to the Email ActionResult in the ContactsController.
2.	When the user submits this data, the input should be validated against the following rules. Any validation errors should be presented to the user
a.	The Validation was working for the first and Last name in the project but not for the email. I followed the documentation for email validation, I had email validation working when I moved over to a personal project.
3.	All data submitted in this way must be saved, but only for the duration of the application’s run. It does not need to survive a restart of the application. However, in your design consider that this application will ultimately have to save this data to a persistent datastore.
a.	I attempted to save data through both session storage and TempData. Both worked for a single entry, but when assigning to a list I was unsuccessful to loop through it with either a for or a foreach loop. But that is how I would store the information without a database and persist across multiple Views in the same session. 
4.	A REST endpoint must be provided to retrieve all mailing list entries. This endpoint should take 2 optional parameters:
a.	I was able to successfully use the Get and Post Endpoints.
5.	Last name- if specified, only records with this last name are returned
a.	I was unable to get to this task in time but If I were to do it, I would use jquery and filter by #id.value
6.	Ascending/Descending flag which indicates how to sort records. If not specified, default behavior is to sort ascending. Records should be sorted by last name. Where last names are equal, records should be sorted by first name.
a.	I was unable to get to this task – If I were to complete this task I would fetch the list of contacts like so: var listVar = list.OrderBy(x => x).ToList() for ascending
7.	At least one automated test must be provided which tests one of your .net components.
a.	I was unable to get to this task.

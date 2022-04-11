Solution Name:- Demo.TripService
1.	Demo.TripService.API :- Web API project which will Create and Get a trip and Save and fetch from the  cosmos 
2.	Demo.TripService.Domain :- Holding Common model and Repositories services 
3.	Demo.Azure.Services :- Cosmos DB Generic methods 
4.	Demo.Trip.EventSender :- Window application which will raised the event 
5.	Demo.Trip.EventReciver :- Event listener and storage device vent into database
6.	Demo.Azure.Services.Tests :- Unit Test project 
7.	Demo.TripService.API.Tests :- Unit Test Project


 
Flow :-
1.	Create Trip :- Create Trip end point create a trip which will accept Trip Request input parameter and return trip Id.
2.	Get Trip :- Return Trip details based on trip Id
3.	Demo.Trip.EventSender :- pushing trip details into event hub 
4.	Demo.Trip.EventReciver :-Event hub trigger azure function read device event from event hub and stored  into database 
5.	Get Trip :- UI will call after serval interval and display the coordinates 

Note: - Challenges 
1.	Due to firewall issue on my machine unable to access azure service and end to end functionality testing  

# Fleet Tracker

# Technology: Microsoft .Net, Geolocation Googleapis, Sql Server LocalDb

# Database Model:  Entity Framework Code First, Fluent Api, Repository, Unit Of Work

# Entities:

- Driver: Store information about the drivers
	Id (PK), Name


- Vehicle: Store information about the vehicles 

	Id (PK), Name


- Freight: Store information about the freight

	Id, Description, Date, VehicleId (FK), DriverId (FK) 


- TrackingCurrentPosition: Store current position of each freight

	Id, FreightId (FK), Description, Lat, Lng 


- TrackingCurrentLog: Store historical position of each freight

	Id, FreightId (FK), Timestamp, Lat, Lng


# Database Access:  .Net Web Api

# Security: Asp.Net Identity / Json Web Token 

# Front End: Asp.Net MVC, Google Maps, HTML Geolocation

# Instructions:

1- Extract the files in a new directory (if you prefer, clone it in the GitHub - git clone https://github.com/maabreve/fleet-tracker)
2- Open the solution FleetTracker.sln in Visual Studio 
3- Build and Run the solution (Ctrl + F5) (Confirm if the project FleeTracker.Web is the startup project)
4- Register a new user
5- Click on the map locations to see freight details

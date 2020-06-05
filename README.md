# Take-home Assignment: MovinOn

![N|](https://www.mcgill.ca/research-jobs/sites/all/themes/moriarty/images/logo-red.svg)


Professor: Khattar Daou
Student: Lucas Napoli / Phillip Spencer-Boucher
Development: MovinOn

# Purpose of the database
## Tracking the operations of MovinOn. Mainly logistic and rental operations. 

Database should be designed thinking in the data flow process taking in to consideration the main data entries processes: **Job Management**,**Rental Control**, **Clients**, **Employees**, **Drivers**  and **Warehouse**. For that reason, some work flows has been taking into consideration:
1. Employees
2. Clients 
3. Vehicles 
4. Jobs
5. Rentals
6. Warehouse
7. Units


# Assumptions: User's Stories 

Some assumptions are important to design the database:
1. Credentials management tables are not required.
2. Logical deletion will be implemented to avoid delete records.
3. Control fields are not required.
4. Business rules will be implemented in other layer.
5. We are going to work with states (in-progress, completed, etc) in the cases of jobs and Rent.


# LookUp Tables Normalization

1. Normalization table (LookUpLocation) was implemented to normalize: country, postalCode, region, city. Categories will use to filter by the field requested. 
2. Status were normalized y managed based on the case: Jobs or Rent. 


# Other considerations
1. Record managed by date to keep the track of the changes.
2. Logic deletion is implemented with a boolean datatype.


# ER Diagram

![N|](Pics/MovingOn.png)


# License
----

MIT
**Free Software**
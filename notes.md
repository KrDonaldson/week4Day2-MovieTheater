<!-- Each employee and customer may have address information and contact 
information. This information can be obtained from the address table or contact 
table. Since one person’s contact and address information can change, these 
tables are connected to the employee and customer tables with the respective ids

Employee: each employee will have an address, contact information, role and 
first and last name. The role can be changed/updated and multiple employees can 
have the same role. The role will be connected to the employee’s information via 
the employee_role_id.

Categories: 
Each movie can have multiple categories, and each category can apply to multiple 
movies, so both a category table and a linking table, movie_catagory, was 
necessary. 

Rating:
Most movies only have one rating based on the chosen rating system (PG, PG-13)

Movie: Each movie will have a title, one rating, a description, a language (id 
is based on the language code), length, cost, and may have multiple categories. 

Ticket: One movie per ticket, customer can have multiple tickets
    Going further: attaching a ticket to a showing category, such as matinee, 
    premium, etc to adjust the cost of the ticket based on the start time

Concession: 
There are multiple concessions to choose from, multiple concessions can be in 
one cart, and many different carts can have the same concessions, as each 
concessions’ inventory is theoretically more than one, so a concession table and 
cart_concession linking table are necessary. 

Order & Cart: a customer can purchase concessions without purchasing a ticket 
and a ticket can be purchased without purchasing concessions.The Order table 
will need to connect to the ticket. The Cart table will need to connect to the 
cart_concession. Both Order and Cart will need an employee, a customer, and a 
timestamp. 

Payment: Based on the rules for order and cart, the payment needs to allow both 
the cart)id and order_id to be null. It will still have a customer id and 
employee id. There should also be a total cost based on their purchases as well 
as a payment timestamp. 
	Going further: would include adding a payment type table -->

<!-- Note: I used SqlDBM for the entity relationship diagram (ERD) and could 
not locate how to adjust the cardinality images, so that would be a Going 
Further item-->

<!-- DB created with ElephantSQL -->
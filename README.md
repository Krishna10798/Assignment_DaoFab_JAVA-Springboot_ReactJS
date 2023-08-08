# Assignment_DaoFab_JAVA-Springboot_ReactJS
This multifaceted assignment assesses your frontend and backend skills using two JSON files: Parent.Json and Child.Json. It involves creating a paginated parent transaction table with sorting, calculating Total Paid Amount. A new page displays child installment data



Coding Assignment for DAOFAB
This coding assignment is to gauge both your frontend and backend capabilities. 
This assignment consists of two accompanying JSON files (Parent.Json and Child.Json) containing JSON data. 
Parent.json
The main data in this file is an array of json objects. 
Each object represents a transaction information.
Each object contains the following values:-
•	id –database row id
•	sender – sender’s name/id
•	receiver – receiver’s name/id
•	totalAmount – total amount to be paid for a transaction
Child.json
The main data in this file is also an array of json objects. 
Each object represents an installment payment and contains the information about the amount paid for each installment.
The object contains the following values:-
•	id – child’s id
•	parentId – parent transaction id (this corresponds to the id in the Parent.json)
•	paidAmount – amount paid in this installment
Note: 
•	Not every parent object will have a corresponding child id (e.g. child id/object is non-mandatory)
•	A parent object may also contain multiple child ids.
Tasks
For your first task, you are required to create a table to display all the parent transactions (contained in Parent.Json). 
Details:-
Implement a REST API to fetch data build server-side pagination. Each page should display 2 rows (with a pageSize of 2) and be capable of being sorted by the parent id. 
The Parent table shall contain the following columns - Parent id, Sender, Receiver, Total Amount and Total Paid Amount (Sum of all paid amounts in the corresponding installment/child id – See below).
Sample :
ID	Sender	Receiver	Total Amount	Total Paid Amount
1	ABC	XYZ	200	100

For your second task:- When the user clicks, Total Paid Amount, display a new page and populate the corresponding children (installment) data.
Details:-
Implement a REST API to fetch child data. 

The Child table shall contain the following columns – Child id, Sender, Receiver, Total Amount and Paid Amount (amount paid in that particular installment). Populate all data sorted by id (no pagination required).
Sample:
ID	Sender	Receiver	Total Amount	Paid Amount
1	ABC	XYZ	200	10
2	ABC	XYZ	200	50

Commit your code to a Github repository and share the link with us upon completion. Please provide adequate comments in your code to provide for readability.


output-
Parent Transactions
ID	Sender	Receiver	Total Amount	Total Paid Amount
1	ABC	XYZ	200	Click to view Child data
2	EFG	PQR	300	Click to view Child data
Child Installments for Parent ID 1
ID	Sender	Receiver	Total Amount	Paid Amount
1	ABC	XYZ	200	10
2	EFG	PQR	300	50
in tabular form.

# Inventory Management
An assignment to produce a simple inventory management system using google colab or jupyter notebook.

## DataBase
NoSQL database was used and for handeling and recording data JSON files are used.

* json.loads() : we used json.load() which convert string data read from JSON file to string.
* json.dumps() : json.dumps() was used to converts dictionary objects of Python into  string data format.
* read  and write functions were also used to check and update inventory.


## JSON Files
There are Three  JSON files 

* record before sale.json : In this file we contain all the data of the products in inventory after adding products.
* record after sale.json : In this file we contain all the data of the products in inventory after selling products.
* sales.json : In this file we store the data of products sold.

## ipynb files & there functions

**Adding_products**
* This is used to add products to inventory
* No. of products to be added is asked and for loop is used to add all the products.
* If product id is present in  the inventory, the quantity of that particular product will increase by the amount added to inventory.
* if product is not present. it is added to the inventory with its id.
* all these processes are updated in JSON file.

**Purchasing_products**
* This ask user for product id and quantity he want to buy. 
* If product id is present in inventory record further processing is done else **"INVALID PRODUCT ID" "PLEASE ENTER A VALID ID"** is shown.
* If quantity asked is less then or equal to that in inventory sale is done and info about product and billing amount is shown.
* If quantity is greater then in inventory. Quantity in inventory is shown and user is asked to enter quantity less or equal to that.
* If user enter valid quantity sale is done else a message is shown saying **"ORDER CANCELLED"**.
* After sale the quantity is removed from inventory record and a new recod of sale is made.

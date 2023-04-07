# ShoppingList

A RPA app developed with UiPath Studio that emails the user the optimal shopping list based on different criterias

### Description

---

The app serves as a personal assistant for a daily task of searching products based on different criterias. The user emails the robot the list with its items to be searched and it will recive as a reply the list with the optimal shopping list (the cheapest that meet the criteria). Morover, the products will be added to users wishlist, ready to be purchased.

### Workflow

---

1. The Robot checks daily its email adress and downloads the recieved messages;
2. It reads the data from the PDF attachment (the list of needed items and the criteria of choice - cheap/expesive/relevance/discount);
3. The search beggings successively on websites (Altex & Emag):
  3.1. Log in is perfomed with user creditentials - stored remote on UIPath cloud service;
  3.2  Each item from the shopping list is searched, for each one the robot chooses the best article based on the given criteria, adds it to users' wishlist and stores the price and the link in an Excel document;
  3.3. The user is logged out;
4. The final list is made by comparing the best products from each site and choosing the cheapest one;
5. The robot emails the list of products to the user.

🚲 Bike Rental System (Python)
This Python program simulates a Bike Rental system. It allows users to rent bikes, return bikes, and calculates the rental bill based on the rental basis (daily or weekly). It also applies discounts for rentals within a certain duration.
________________________________________
🎯 Features
  •	Rent Bikes: Customers can rent bikes from the shop based on availability.
  •	Return Bikes: Customers can return rented bikes, and the stock is updated accordingly.
  •	Bill Calculation: The total rental bill is calculated based on the number of bikes, rental basis (daily or weekly), and the rental duration.
  •	Discount Application: A 30% discount is applied for rentals between 3 to 5 days.
  •	Stock Management: The available stock of bikes is managed automatically.
________________________________________
🛠️ Requirements
  •	Python 3.x  (Compatible with any version of Python 3.x)
________________________________________
🚀 How to Run
  1.	Clone or Download the repository.
  2.	Ensure you have Python 3.x installed on your system.
  3.	Open a terminal and navigate to the folder containing the script.
  4.	Run the script using:
        python bike_rental.py
  5.	Follow the prompts to rent or return bikes.
________________________________________
🧠 Code Explanation
1. BikeRental Class
   The BikeRental class manages the bike stock available for rent. The class has:
    •	stock: A class variable that tracks the number of bikes available.
    •	display_stock(): A method to display the current stock available.
2. Customer Class
  The Customer class extends the BikeRental class and simulates customer actions such as renting and returning bikes. The class contains:
    •	rent_bike(): Method for renting bikes. It checks if enough bikes are available and updates the stock.
    •	return_bike(): Method for returning bikes. It updates the stock and calculates the total rental bill based on the rental basis and rental duration.
3. Bill Calculation
  •	The bill is calculated based on the number of bikes and the rental duration (in days or weeks).
  •	A 30% discount is applied if the rental duration is between 3 and 5 days.
________________________________________
📚 What I Learned
While working on this project, I learned:
  •	How to use inheritance in Python by creating a subclass (Customer) that extends the BikeRental class.
  •	How to implement stock management for a rental system using class variables.
  •	How to calculate bills based on different rental types (daily or weekly) and how to apply discounts for eligible rentals.
  •	Best practices for handling user input and maintaining clean code structure.
________________________________________
🚀 Future Enhancements
  •	Add validation to ensure the rental period is entered correctly.
  •	Store the rental data in a file (e.g., JSON, CSV) for persistence.
  •	Allow customers to choose their bike types (e.g., mountain, road, electric).
  •	Implement a logging system to track rental activities.


💻 Example Usage
# Example usage of BikeRental and Customer classes
  bike_rental_shop = BikeRental()
  bike_rental_shop.displaystock()

# Customer 1: Renting and returning bikes
  customer1 = Customer(3, 'daily', 4)
  customer1.rentBike()
  customer1.returnBike()

# Customer 2: Renting and returning bikes
  customer2 = Customer(5, 'weekly', 2)
  customer2.rentBike()
  customer2.returnBike()

  
Example Output:
    Welcome to rental bike shop
    Stock available 100
    3 Stock available 97
    3 Stock available 100
    Your Total bill will be: 1200
    You are eligible for Family rental promotion of 30% discount that is: 840.0


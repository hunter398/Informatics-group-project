# Informatics Project Design

This is essentially where we will plan more on how to implement the Project.

Input
o	Marks - textbox
o	Number of Days - textbox
o	Price per Kilo of SPF – textbox
o	Details of each puppy - Inputbox


Output
o	Details of puppy      -     grid
	Name
	Weight each day
	Total food feed 
o	Total Food for all puppies – textbox
o	Total money spent – textbox


Events	Action
btnSetup	Read number of days and puppies. The price per kilo of food. 
Resize the array
Resize the grid
Create the objects of each puppy
btnReadinAndDisplay	Read details of each puppy and display name and weight to each puppy to the grid
btnDeterminetotalFoodperPuppy	Determine the total food per puppy each day and total overall. This information will then be displayed
btnTotalFoodandCost	Determine the total kilo need and the cost to be display in textboxes.

Variables
•	numDays – Integer
•	numPuppies – Integer
•	PriceperKilo – double
•	Puppies() – puppy
•	d - Integer
•	p  - Integer

Interface







Algorithm 
btnSetup
	Read in the number of puppies, days and price per kilo of food through textboxes
	Resize the puppies(numPuppies)
	For each puppy
		Create a new object – Puppies(p) = new Puppy(numDays)
	Resize grid to match display of name , weight and total
btnReadinAndDisplay
	for each puppy
		Read and store in name, gender, breed age
		Display the name inn grid
		For each day 
			Read and store the weight of the puppy
			Display the weight of the puppy each day in grid
		Next
	Next
btnDeterminetotalFoodperPuppy
	for each puppy 
		total = Puppies(p). FoodConsumed()
		Display total in the grid
	Next
btnTotalFoodandCost
total = 0 
for each puppy
	total += puppies(p). FoodConsumed()
next
total = total / 1000
Display the total food eaten
Kilo += Cint(total /1000)
If (kilo mod 1000 > 0) then
       Kilo += 1
End if
TotalPrice = Kilo * PricePerKilo
Display total Price

UML Class Diagram 
Puppy
-	_Name: String
-	_Breed : String
-	_Gender : String
-	_Age : Double
-	_Weight[1…*]:Integer
<<Constructor>>
+ Puppy(numdays:Integer)
<<Property>>
+Name():String
+Breed():String
+Gender():String
+Age():Double
+Weight(index:Integer) : Integer
<<Methods>>
+FoodConsumed(): Double


 


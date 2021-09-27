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
btnLearn
	Read in topic choice
	Display Learning Material
btnQuiz 
	Generate random questions with answer
	for each question	
		display problem
		read in input
		if answer is correct
			display correct
		else
			display correct answer
		end if
	end for


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


 


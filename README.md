# CarpetCostEstimator
In this question you will write a class called CarpetCostEstimator which models a cost estimator for a carpet shop supplying and fitting carpet. The class has 3 instance variables:
•	price, the price of the carpet in £ per square metre as a double,
•	labourCharge, the labour charge in £ per square metre as a double,
•	postCode, the customer’s postcode as a String (used to determine a price multiplier for expensive areas).
You will write methods to calculate and display the cost of fitting a carpet, given its width and length and the customer’s postcode.

•	A).Launch BlueJ, open the project TMA01_Q1 in the TMA01Download folder you unzipped earlier and then immediately save the project as TMA01_Q1_Sol, in the TMA01Download folder. This doesn’t contain any classes yet.
Next create a class called CarpetCostEstimator in this project. You will develop this class in the following parts.
In the class that is created, delete the example instance variable, the line of code in the constructor that assigns 0 to the variable, and the sample method. Also remove any comments related to the variable and the sample method.
Retain the class comment but edit to it include your own name and the date. For the description of the class write ‘Answer to TMA01 Question 1’.
Paste the whole class so far into your Solution Document.
(1 mark)

•	B).In the class CarpetCostEstimator:
o	i. Declare the three instance variables using the names and types specified earlier.
o	ii. Edit the constructor for CarpetCostEstimator so that it takes a single double argument and sets the instance variable labourCharge to the value of this argument, and sets price and postCode respectively to -1.0 and “XXX XXX”.
o	iii. Write getter and setter methods for price, labourCharge and postCode.
Compile your class and then create an object of the class CarpetCostEstimator in the OUWorkspace, passing it the value 4.0 for the labour charge. Test your getter methods by sending an appropriate message to your object and checking the output in the Display Pane. If you are not sure how to do this test please see the first two lines of test code in the project README.TXT file for example test code. In the test code, we used the identifier cce for our CarpetCostEstimator object.
Include a screenshot of the workspace showing your completed tests in your Solution Document.
(5 marks)

•	C).In this part you are going to write two instance methods to calculate the purchase cost of the carpet as well as its fitting cost. These methods should be private as they are helper methods but you can make them public for the purpose of the question to aid testing.
o	i. Write a method calculateCarpetCost() that takes two int arguments representing the width and length in metres of the carpet to be purchased and returns the cost of the carpet as a double. It should first calculate the area of the carpet then multiply this by the price.
o	ii. Write a method calculateFittingCost() that takes two int arguments representing the width and length in metres of the carpet to be purchased and returns the fitting cost of the carpet as a double. It should first calculate the area of the carpet then multiply this by the labourCharge.
(3 marks)

•	D). In this part you will write a method that uses the postCode to create a multiplier for the labourCharge to increase this for expensive areas.
o	i. Write a public method costMultiplier() that takes no arguments and returns a double. The method should return 1.2 for postcodes beginning “WC1A” or “EC1A”, and 1.0 otherwise. Don’t forget to test your method in the OUWorkspace using various postcodes.
o	ii. Should costMultiplier() be public or private? Briefly explain your reasoning.
o	iii. Amend your calculateFittingCost() method from part (c)(ii) so that it multiplies the labour cost by the appropriate cost multiplier.
Important: you will need to use String methods such as substring() for this part. You’ll find these documented on pp. 18 - 21 of your Exam Handbook.
About the Exam Handbook: You are allowed to annotate the Exam Handbook and take it into the exam with you. However, we strongly recommend that you do not begin adding annotations at this point, because you may clutter your handbook up with facts which it turns out later you don’t really need. When it gets nearer to the exam, you will be in a much better position to decide which annotations you are going to find most useful.
(6 marks)

•	E.In this part you will write a method printCostTable() that prints out a table like the following:

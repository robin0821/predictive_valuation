# predictive_valuation
Predictive valuation on residential property in metropolitan Melbourne
Objective
The exercise aims to get indicative prediction of valuation on residential property in metropolitan Melbourne areas i.e. when details of property such as property type, land size, number of bedrooms, etc. provided, it would be able to provide an indicative valuation of the property. Ideally, the indicative result will be more robust than most of ready products in marketplace. 
The valuation system will comprises two ends – front end and back end. In the front end (UI), it will be a web based service where users can input information for the property that they would like to evaluate. In the back end, a machine learning based computer algorithm is expected to be the corner stone of the system.
Machine learning algorithm
-	TBD
Steps
1.	Get data ready
a.	Get past transaction data i.e. price, property type, date sold, land size, number of bedroom, number of bathrooms, number of parking spaces, detailed address.
b.	Get school data i.e. school name, address, location (latitude, longitude), rank.
c.	Get railway station data i.e. location (latitude, longitude)
d.	Get suburb shopping centres data i.e. location (latitude, longitude)
e.	Compile data above into one dataset for modelling
2.	Test and refine modelling
Based on rules of thumb, the main drivers for residential property include factors below:
•	Location – is the property close of CBD?
•	Educational resources – is the property located in good public school zone?
•	Transportation friendliness – is the property close to railway station? Bus and taxi access are excluded as they are presumably evenly distributed across metropolitan Melbourne area.  
•	Living friendliness – is the property close to main shopping centres which scattered across metropolitan area of Melbourne?
Ideally, a robust predictive modelling should incorporate all factors above. However, the level of effort will dramatically change with some factors into conclusion such as railway station data and shopping centre data preparation. Hence, a step-wise approach would be more favourable in essence i.e. build a simpler modelling with partial of the factors at first to test the robustness of modelling. Only should other factors included when the results wouldn’t meet expectations. 
•	Step 1 – modelling with location and educational resources
•	Step 2 – modelling with location, educational resources and transportation friendliness
•	Step 3 – modelling with all main factors
Goal is supposed to be accomplished at any step where desired accuracy is achieved. 
3.	Deploy the front end (UI)
The UI should be modelling agnostic i.e. end users should be easily navigator the interface without any hassle to have a quick valuation assessment of their properties. To meet this target, some below requirements are to be met:
•	Web based service
•	Minimal inputs of info – only information such as land size, number of bedrooms, bathrooms, parking spaces and detailed address to be input. The back end should be able to convert the address to location automatically and do other calculation such as educational resources, and living friendliness without being noticed
•	Self-maintenance – the system should be able to download the new transactional data on weekly basis without manual interference to make the modelling up to date. (this can be included in future version)
•	Mobile app (this can be included in future version)



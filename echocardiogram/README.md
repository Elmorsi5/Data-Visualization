###Purpose:
#to classify if patient will live at least one year after a heart attack.Steps of Solving:
	* #Well Understanding the Data.
	* #Cleaning and make data ready to be visualized.
	* #ML(KNN applying).

##3Well Understanding the Data:
#i will reset columns name to be easier to be understood and visualize which isn't useful anymore
	1. #survival : number of months the patient had lived-he may be dead or still alive, so check the next factor-.
	2. #still-alive: 0=dead, 1= alive
	3. #attack_age: how old he was when he had been attacked
	4. pericardial_effusion: we are searching for the fluids around the heart, if there is a fluids=1, no fluids=0
	5. fractional-shortening: a measure of contracility around the heart, lower numbers are increasingly abnormal
	6. epss: E-point septal separation, another measure of contractility-it is measure the amount of movement of the muscle towards the septum-normal is <=7,Larger numbers are increasingly abnormal
	7. lvdd : left ventricular end-diastolic dimension.  This is a measure of the size of the heart at end-diastole
	8. wall-motion-score: we will replace it with next factor
	9. wall-motion-index: equals wall-motion-score divided by number of segments seen.  Usually 12-13 segments are seen in an echocardiogram
	10. mult : we will not use it anymore
	11. name : the name of patient but it's not usefull yet as all names are written as 'name'
	12. group :usless
	13. alive_at_1: the patient still alive after 1 year or not, if 0= dead , 1=alive

Columns=['survival','still-alive','attack_age','pericardial_effusion','fractional-shortening','epss','lvdd','wall-motion-score','wall-motion-score'wall-motion-index','mult','name','group','alive_at_1']Cleaning and make data ready to be visualized[x]Rename Columns[x]Take a look For the Data[x]Remove useless columns[x]Turn '?' into NaN[x]Drop some useless rows[x]reset the index[x]fix the missed Values in the 'alive_at_1' as it depends on the 'survival' column[x]Fill the missing data with avg if it's possible[x]Take a look about the info to make sure of the data Type[x]if a column type need to be changed we will do itVisualizing Data
[x]Count the value in rows
[x]trying to find relations between the whole factors
[x]use different kind of plots even if it may be meaningless:"

ML(KNN applying)
[x]split dataset to model data(x) and our target(y)
[x]split between training and testing be 20:80
[x]Feature scaling
[x]  Define our model with different values of k to get the best accuracy score
[x]define the maximum value between them

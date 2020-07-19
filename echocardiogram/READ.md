### echocardiogram

## Purpose
 to classify if patient will live at least one year after a heart attack.
 ## Steps of Solving:
  - Well Understanding the Data.
  - Cleaning and make data ready to be visualized.
  - ML(KNN applying).
	
  ## Well Understanding the Data:
  ```python
  #at first i will reset columns name to be easier to be understood and visualize which isn't useful anymore
  Columns=['survival','still-alive','attack_age','pericardial_effusion','fractional-shortening','epss','lvdd','wall-motion-score','wall-motion-score'wall-motion-index'
,'mult','name','group','alive_at_1']
```
 
	1. survival : number of months the patient had lived-he may be dead or still alive, so check the next factor-.
	2. still-alive: 0=dead, 1= alive
	3. attack_age: how old he was when he had been attacked
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
  
## Cleaning and make data ready to be visualized:
  - Rename Columns
  - Take a look For the Data
  - Remove useless columns
  - Turn '?' into NaN
  - Drop some useless rows
  - reset the index
  - fix the missed Values in the 'alive_at_1' as it depends on the 'survival' column
  - Fill the missing data with avg if it's possible
  - Take a look about the info to make sure of the data Type
  - if a column type need to be changed we will do it

## Visualizing Data:
  - Count the value in rows
  - trying to find relations between the whole factors
  - use different kind of plots even if it may be meaningless:"

## ML(KNN appalying):
  - split dataset to model data(x) and our target(y)
  - split between training and testing be 20:80
  - Feature scaling
  - Define our model with different values of k to get the best accuracy score
  - define the maximum value between them

## Resource:
[DATA](https://data.world/uci/echocardiogram?fbclid=IwAR119-0JSPswIykX5IhmFOIueuB6VHOfQow6KTzWbyn-7UIVW7LYkKvbLv8)
### Vidos can help you well understand
   - [Video1](https://www.youtube.com/watch?v=PQ8bMAxjxRk)
   - [video2](https://www.youtube.com/watch?v=dciFRAawP1o)
   - [video3](https://www.youtube.com/watch?v=buiH2hfLoEg0)




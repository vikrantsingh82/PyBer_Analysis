# PyBer Analysis using Pandas and Matplotlib

## Overview of the analysis

Using Python skills and knowledge of Pandas, we need to create a summary DataFrame of the ride-sharing data by city type by 
- Total Fares
- Total # of ride and drivers
- And average fare per ride and driver respectively . 

Then, using Pandas and Matplotlib, we’ll create a multiple-line graph that shows the total weekly fares for each city type

## Results

### Deliverable 1 : A ride-sharing summary DataFrame by city type
For this we read the data from CSV files (City_data.csv and Ride_data.scv) into two respective dataframes and then merged both these into one dataframe.

![image](https://user-images.githubusercontent.com/98173091/156969920-61afe265-7468-4b58-b5a3-f0082cbe9271.png)

Merging the two dataframes

![image](https://user-images.githubusercontent.com/98173091/156969996-932cb0b8-51d1-4cff-a61e-84e6c17a0aea.png)

Reading the Urban, Suburban and Rural type city data in respective dataframes and then uinsg the groupby fucntion Total Fare, # of drivers and ride for each city type are stored in variables. 

![image](https://user-images.githubusercontent.com/98173091/156970190-84f07206-c935-4724-97b0-8e507e21dfd1.png)

![image](https://user-images.githubusercontent.com/98173091/156970231-8565b9a1-716c-40e4-9366-b85ca96793be.png)

![image](https://user-images.githubusercontent.com/98173091/156970282-934297fa-c4d6-4e73-bf18-c3e5c6ea5519.png)

![image](https://user-images.githubusercontent.com/98173091/156970316-bcc0e146-b2e8-4fce-8ade-c9c4e42fb763.png)

Average Fare per driver and ride

![image](https://user-images.githubusercontent.com/98173091/156970378-c55ccdb0-69e4-4aba-bd7f-4fd9f9969f4a.png)

![image](https://user-images.githubusercontent.com/98173091/156970418-62779eaa-7ddb-47ff-9574-b30c46effae6.png)

#### Creating Series for each city type for calculated statistics 

![image](https://user-images.githubusercontent.com/98173091/156970503-bda7484a-702a-4dba-926d-39dc672bebb6.png)

#### Creating and formatting the new summary dataframe usinge the series created above

![image](https://user-images.githubusercontent.com/98173091/156970630-d9473fa1-d35c-4c5a-ae36-f7876aca370d.png)

![image](https://user-images.githubusercontent.com/98173091/156970661-bced0902-a0bb-444b-ad34-9ff8d313f00c.png)

Formatting the dataframe

![image](https://user-images.githubusercontent.com/98173091/156970707-968fb035-0906-497e-a672-935350d545c9.png)

### Deliverable 2 : A multiple-line chart of total fares for each city type
Reading the merged dataframe

![image](https://user-images.githubusercontent.com/98173091/156970846-686d9045-49c8-4d1c-b13f-db00c76e837a.png)

Using group by function to create new dataframe for showing sum of fares for each city type

![image](https://user-images.githubusercontent.com/98173091/156970978-8f366ae8-3488-4b5f-af96-5c378894b7dd.png)

Resetting index on the newly created dataframe and creating a PIVOT table

![image](https://user-images.githubusercontent.com/98173091/156971292-b58903fa-043e-45dd-a6a7-d0679519dd35.png)

Filterin the pivot table for dates '2019-01-01':'2019-04-29'

![image](https://user-images.githubusercontent.com/98173091/156971415-32d7937e-ac0b-4798-a951-2140b757e273.png)

Converting the pivot table dataframe's index to datetime type

![image](https://user-images.githubusercontent.com/98173091/156971486-6313e961-a383-432f-b976-116cf8a18af8.png)

Using the resample function, we created a new DataFrame by week and get the sum of the fares for each week

![image](https://user-images.githubusercontent.com/98173091/156971550-7800d1bb-4720-4959-8dd9-552c8f66f9cc.png)

Using the resampled weekly data for dates (2019-01-01 to 2019-04-29) we platted a line graphs showing the lines for each city type

![image](https://user-images.githubusercontent.com/98173091/156971737-6126f394-707c-4648-bea4-b3f9c3180434.png)

![image](https://user-images.githubusercontent.com/98173091/156971772-6ef07039-0568-45fb-ad53-85265221d05e.png)







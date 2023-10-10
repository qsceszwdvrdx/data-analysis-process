# Spaceship_Titanic
kaggle Competitions data : [link](https://www.kaggle.com/competitions/spaceship-titanic)

code referene : [link](https://www.kaggle.com/code/computervisi/best-models-spaceship-titanic)

Target : The topic is similar to Titanic, using the features in the data to find out which people will be transported.

The process is divided into 4 parts, namely EDA / fill null / models comparison / models predict


## 1.EDA
>Preliminary exploration of raw data.

raw data : 13 features & 1 label (transpored)

|feature name|description|handle|
|------------|---------|-----------|
|PassengerId |Each Id takes the form gggg_pp where gggg indicates a group the passenger is travelling with and pp is their number within the group. People in a group are often family members, but not always.|Divided into groups and numbers within groups.and calculate the group size and whether it is single person|
|HomePlanet  |The planet the passenger departed from, typically their planet of permanent residence. |        |
|CryoSleep   |Indicates whether the passenger elected to be put into suspended animation for the duration of the voyage. Passengers in cryosleep are confined to their cabins.|        |
|Cabin       |The cabin number where the passenger is staying. Takes the form deck/num/side, where side can be either P for Port or S for Starboard.|Divided into deck, num and side|
|Destination |The planet the passenger will be debarking to.|        |
|Age         |The age of the passenger.|compare each age group|
|VIP         |Whether the passenger has paid for special VIP service during the voyage.|        |
|RoomService |Amount the passenger has billed at each of the luxury amenities.|Add up the additional costs and compare the distribution of each payment, as well as the proportion of whether there is payment or not.|
|FoodCourt   |Same as mentioned above.|Same as mentioned above.|
|ShoppingMall|Same as mentioned above.|Same as mentioned above.|
|Spa         |Same as mentioned above.|Same as mentioned above.|
|VRDeck      |Same as mentioned above.|Same as mentioned above.|
|Name        |The first and last names of the passenger.|drop irrelevant features.|
|Transported |Whether the passenger was transported to another dimension. This is the target, the column you are trying to predict.|        |

Visualize the difference between each feature and whether it is transported.
There is a method on kaggle to use last name, but I choose not to use it.

## 2.fill null 
>If there are highly correlated features in the existing data, fill missing values with the nearest available numerical values.

## 3.models comparison
>Compare the model's performance, runtime, and accuracy.

## 4.model predict
>Input the data into the model for prediction. Select the top five models based on accuracy for individual testing and comprehensive evaluation.

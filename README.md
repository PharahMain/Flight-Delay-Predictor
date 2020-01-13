# Flight-Delay-Predictor
Research Proposal: Flight Delay Predictor
At any given time, 10,000 vessels made of aluminum and carbon composite material weighing more than 150,000 lbs are hurling through the air tens of thousands of feet above our heads carrying more than a million passengers. In just over a century, aviation has made leaps and bounds in safety and reliability that, for some of us, biggest worry is whether there will be a baby onboard on your flight whether we care to admit it or not. But I think, we air travelers can agree on how we feel about delays, be it on the tarmac or in the gate. And the range of emotions can scale from mildly annoyed to enraged depending on the length of the delay. I theorize that the main source of the frustration stems from not knowing how long the delay might last. That is to say, the difference between expectation and reality is directly correlated to the level of frustration. This will be the main focus of my research. I want to build a model that predicts the length of delay for any given flight scheduled in the near future. Setting the right expectation allays the traveler's stress which will more likely result in repeated business.

As you can see from this graphic from Bureau of Transportation Statistics, aircraft arriving late and air carrier delay are the two largest factors of flight delays.

Data Sources
I will be using two apis: FlightStats and Dark Sky. FlightStats api will give me all relevant information such as departure time and destination and Dark Sky will provide the hourly weather data based on the location of the airport. The data will be merged together into a single dataframe from which I will be building the models.

Techniques
I will be using Google Colab notebook to make the api calls and the data returned will be stored in Google Drive. Once all desired data is gathered, I will build a model using Apache Spark in batch mode. This will then be compared with different models built from using the Scikit-Learn library to pick the most accurate regression model. Time permitting, I will also build/integrate a time series model.

Challenges
On a cursory glance, I think the biggest challenge will come from using two different apis and merging the two sets of data into one and cleaning the dataframe.

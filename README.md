# *Jack's GTA HIKE*

# Introduction/Business Problem

Jack Murphy is a unique character and a successful business owner in the ‘entertainment and adventures’ industry. He has a hiking business across many cities in the US and has decided to open a branch of it in the GTA. He is oscillating between these two boroughs: Scarborough and Etobicoke. Jack is unsure of the neighbourhoods within. He has certain criteria he would like to ensure are met, and the location that most satisfies these requirements will be his choice to lease in. 
Jack, and two employees from marketing/advertising, will be reviewing this report, and the accuracy of the story told by the data provided will be used in advertising the launch of Jack’s GTA Hike. This information may continue to be used in future marketing and advertising campaigns if evidently successful, to continue attracting customers.
One criteria he would like met, is the presence of hotels. A variety of hotels would be most preferable, and with a wide price range to accommodate his customers' financial abilities. 
Another criteria is the presence of at least one coffee shop that opens early and stays open late. This would be most convenient for his customers who may want a coffee in the early mornings and/or who may want a tea when they get back in the evenings. 
The final criteria is a drugstore, or a convenience store. One that supplies ibuprofen for a headache, a toothbrush, a cold drink or a quick snack.
The customers who sign up for Jack's GTA hike would meet up at the business location where a shuttle bus will be waiting to escort them to one of the hike locations. Customers are responsible for their own accommodation, and morning and evening coffee but Jack’s Hike would provide water, meals and snacks throughout the day.
Jack will use the availability of hotels, coffee shops and drugstores near Jack's GTA Hike in his marketing campaign, and therefore the accuracy of the report is of utmost importance. Jack prides himself in his dependability and accuracy in advertising. He likes to under-promise and over-deliver, so any inconsistencies will be costly to his reputation, and of course, to our reputation.

# Data

I will start by finding the neighborhoods of both Etobicoke and Scarborough, then finding the top venues in each, just for an idea of what I am working with. After listing the venues per neighbourhood in Etobicoke and Scarborough, then compare the selected three venues (hotels, coffee shops and drugstores or convenience stores) within the two boroughs (Etobicoke and Scarborough) and in turn compare neighbourhoods within to determine most suitable locations to Jack's criteria. After finding the neighborhoods that match Jack's criteria the most, I will proceed to compare the hours of operation for the coffee shops from Foursquare. Having narrowed down the selection of neighbourhoods I will then research hotel prices (possibly via an external source) to ensure there is a range of prices available in the remaining neighbourhoods. 
If I run into a situation where it seems these three criteria are not easily met. I will change the order of elimination so that my recommendations vary. So, I may start with the three venues but eliminate by hotel prices before coffee shop operation hours, if I find the need to do so.
I will present the top three neighbourhoods to Jack and his team with supporting evidence from Foursquare.


# Understanding the data

Before proceeding to understand the neighbourhoods within Scarborough and Etobicoke in particular, and since they are boroughs of Toronto, it is best to get a clear idea of all the borough of toronto and map out the neighbourhoods by cluster in Etobicoke and in Scarborough. This gives an idea as to why Jack may have even chosen these two in particular.

## Data requirements

In each Scarborough and Etobicoke we need to collect:
- The neighbourhoods
- The venues in each neighbourhood
After glancing over the output
- Reduce the dataframe to venues that would include coffee shops, stores and hotels
collect venues in Etobicoke and SCarborough 

## Data Collection

First round: collected the data in the venues for Coffee Shops, Stores and Hotels
Second round: went back to my data collection and edited it to collect coffee shops, cafes, stores and hotels
thirs round: went back and realized that stores could be pharmacies or grocery stores
fourth round: went back and included convenience store and deli to the stores

## Data understanding (visualization included)

This step was also run a few times, and finally landed on the following bar graphs that are an excellent summary of the data collected 
Only Clarks' in Scarborough has more than two hotels. We need to check the coffee shop hours and the range of hotel proces still. Woburn and Scarborough Village have 10 more more coffee shops and 8 or more stores, but both these neighbourhoods have only one hotel each, which means that Jack will not have a price range for his customers. 

Kingsview, Northwest and Westmount are the most viable neighbourhoods in Etobicoke as per the bar graph. The remaining three neighbourhoods do not have the same number of options. In the case that the coffee shop hours or the hotel price range do not meet Jack's criteria, we have an option to consider Albion Gardens.

The bargraphs are visible in the code (https://dataplatform.cloud.ibm.com/analytics/notebooks/v2/b8ce6509-68f5-4ba3-8ba2-b3bfe8bc142f/view?access_token=d559e99b4fd6a3800e1361c2f1b4acf1c1c09084fd79579b3d6bad2f1dddb7f5) or on the blog Jack's GTA Hike.


## Data preparation

Data was prepared using wiki for the Toronto postal codes and latitude and longitude, as well as geopy. Matplotlib for plotting the graphs. Clustering neighbourhoods. Foursquare API for requesting venues in locations desired, and premium calls for venue hours of operation, which was needed for coffee shops.

Before deployment, the model will be evaluated by the teams, and feedback will be requested.


# Results

Northwest in Etobicoke and Clark's in Scarborough are the top contenders in each borough. We narrowed it down to the top in each borough as per Jack's request. 

Clarks' has 5 coffee shops, one of which is known to be open 24 hour, 4 stores and 2 hotels! The hotels range in price between $104 and $135

Northwest has 10 coffee shops, 4 stores and 6 hotels. One of the coffee shops was also found to be 24 hours and the hotel prices range from $112 to $135


# Discussion

Jack only asked for these three criteria, therefore even though there are more stores and coffeeshops in other neighbourhoods in Scarborough, we only calculated some coffee shop hours for the hood that had more than one hotel option, espcially since that hood had a price range also as requested by Jack. 
Etobicoke has as many coffee shops and stores, but even upon first glance one can see that it will likely be the ultimate option. 

We were a little side tracked when getting the hours of coffee shops from Etobicoke and finding them open until 10pm whereas Clark's in Scarborough had a Tims open 24hours. Given the limited number of requests to Foursquare premium, I checked a few more coffee shops in Northwest, and voila found a 24 hour coffee shop there too!

# Conclusion
While the price range between the two hotels in Clark's Scarborough is $8 more than the range in prices between the hotels in Northwest, Etobicoke - I proceed to recommend Northwest in Etobicoke as the neighbourhood for Jack's GTA Hike.This neighbourhood provides 3 times as many hotels which range in price just a little less than Clark's hotels. Northwest has a 24hour coffee shop and several stores around for customers' day to day needs.

# gaea_capstone
Gaea Villaroya's economics capstone project

Jon's work:

Step 1: Setup a system for saturating linkedin's legal api for constantly grabbing profile data and pictures given a list of profile IDs e.g. https://developer.linkedin.com/docs/fields/basic-profile
Step 2: Figure out how to get random profile ids from linkedin and do it e.g. https://www.linkedin.com/directory/people-j-100-100-3
Step 3: use stpe1 to query images for photos in the dataset i already have
Step 4: work with haystack's api to upload the photos and download the attractiveness: Authorization: https://api.haystack.com/api/ENDPOINT/ACTION?apikey=3f04d4f03df85960d86885122040b488
Step 5: Merge the haystack dataset with the linkedin dataset and store the results in a new json dataset

Gaea's work:

Parse Jon's dataset in Stata or Python (I recommend Python :P ) and run linear regression on the type of fields you like. I recommend something like X = [float(years of experience), boolean(education has university or college in name),int(number of connections), float(attractiveness)] and Y=[boolean(is currently hired)]. This way, we factor out if the people have lots of experience or education in the decision of if they're hired or not, and with the number of connections we factor that out as affecting beauty (e.g. if someone has 500 connections, then theyre more likely to have a pretty profile pic than if they have 10).

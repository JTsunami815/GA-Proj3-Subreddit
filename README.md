# Project-3: Web APIs & NLP

## Contents:
___
* [Exclusive Summary](#Summary)
* [Context & Background](#Context-&-Background)
* [Problem Statement](#Problem-Statement)
* [Resources](#Resources)
* [Data Dictionary](#Data-Dictionary)
* [Comparison](#Comparison)
* [Conclusion](#Conclusions)
* [Recommendation for the Future](#Recommendation-for-the-Future)
___

## Exclusive Summary
___
Due to COVID-19, these past couple years has caused a turmoil on a lot of adult's mental health.  To the point where it using drinking and/or smoking becomes an addiction.  To help them as well as assist the stakeholders who are looking for a solution, we have developed a tool that will utilize our algorithm to help identify which group the authors can belong to. As well as provide additional assistance to the Stakeholders who belong to non-profit organization. 

This tool will be able to be used in many different digital platform. It will also assist on identifying which group the author of the post belongs to and provide assistance to guide the author to the correct rehabilitation/group/threads/location.
___
[Return to Contents](#Contents)

## Context & Background
___
We are a private company that are looking to assist rehabilitation centers by providing better guidance for the newcoming patients with their addiction by properly classifying them through our designed tool.

With what is going on in the world because of COVID-19, getting access to a physical rehabilitation center to get help becomes harder and harder. People are also finding difficulties to cope with the uncertainty so some of them are using external substance to help with the irregularity in their life. In this case, alcohol and smoking. The range of choice does not matter but the consumption does. To the point where they get addicted to it. To assist those who are thinking to seek help, shelters and non-profit group help companies started to reach out to technological companies to help build alternative tools to help those who need guidance to take the first step to the correct groups to help them improve.
___
[Return to Contents](#Contents)

## Problem Statement
___
To develop a digital tool to assist these organizations who are helping those who have an addiction to either alcohol or cigarrette. By intaking the inputs by the users, our tool will be able to help identify which subreddit the post belongs to through **Train/Test Split, Naive Baynes and K Nearest Neighbors (KNN)**.

A way of engaging patients is to engage them online. Several of them have turned to subreddits in the Reddit website to post about their problems and concerns. By studying this, as well as other platforms in the future, we are able to leverage on this to provide further appropriate treatment to their posts or direct them to the proper out-reach programs.

Our stakeholders has requested us to create an algorithm tool that can quickly and efficiently filter requests from patients who will be using their preferred online platform. This algorithm will be used in their online frontend to quickly identify patients with alcoholism or smoking problems. With this assistance, it will minimising resource and time wastage, allowing help to be rendered more efficiently.
___
[Return to Contents](#Contents)

## Resources
___
**Data:**
* [Alcoholics Anonymous CSV](https://git.generalassemb.ly/jtsunami815/Project-3-Subreddit/blob/master/data/Raw_Alcohol_Anonymous.csv)
* [Stop Smoking CSV](https://git.generalassemb.ly/jtsunami815/Project-3-Subreddit/blob/master/data/Raw_Stop_Smoking.csv)

**3rd Party**
- [Alcoholics Anonymous Singapore](https://www.singaporeaa.org/)
- [Alcohol Rehab Guide](https://www.alcoholrehabguide.org/support/alcoholics-anonymous/)
- [American Lung Assocation](https://www.lung.org/quit-smoking/join-freedom-from-smoking)
- [Stop Smoking Support Program](https://medlineplus.gov/ency/article/007440.htm)
- [Alcoholics Anonymous](https://www.reddit.com/r/alcoholicsanonymous/)
- [Stop Smoking](https://www.reddit.com/r/stopsmoking)
___
[Return to Contents](#Contents)

# Data Dictionary
___
The dictionary table below represents the only columns that are left from the total number of columns.
### Dictionary Key:
___

   |Feature|Type|Dataset|Description|
|- | -|- | -|
|**author**|string|filtered_messages|Author that post within the group|
|**title**|string|filtered_messages|Title text of the subreddit|
|**selftext**|string|filtered_messages|Main text of the subreddit|
|**subreddit**|string|filtered_messages|Subreddit group|
___
[Return to Contents](#Contents)

# Comparison
___
It is clear that our model outperforms our baseline model's R2 score against 55% on the initial base test data. This thus addresses our problem of not having a proper algorithm to classify incoming posts from patients based on the worded text. Our model has a higher level of accuracy in classifying incoming patient's posts with our machine learning model.
___

[Return to Contents](#Contents)

# Conclusion
____
After doing the initial study, we have gained a significant insight on the problems for both sides of the subreddit authors. We can say that each group show an interest on wanting to get help as they personally realise that they do have an addiction. As the first step is to seek help, we think that our tool will be able to assist and guide them as well as th non-profit group to the right direction. By connection the seekers as well as the receivers together online or in person safely, it will be a great stepping stone to the right direction.
___

[Return to Contents](#Contents)

# Recommendation for the Future
__
As this is the beginning stage of our study, we can already say that our tool shows quite a promise as the initial removal of "common" English words we deemed not having an impact and a good indicator shows an improvement compare to using default set of "common" English words. To be able to provide better identify the posts, we will continue to add new post/threads to our machine and see what further actions we will have to do to further improve the system.

Ideas we have as of now is to continue to add more Stopwords to the current list of most common English words used to improve the efficiency (As you can see the difference from Step 4.1 and 4.2). Another is to diverge out from Reddit website and dive into other social media platform that may also use those as a reach out for help. Find tuning our model will also be continue in the future as those can definitely play a factor to the end scores.

We also believe that we can also further tune our tool by implement them to many different platforms. Online and apps are the initial stages where we can allow the end user to key in their story and the system will provide recommendations to their nearby facilities or out-reach programs they can get in contact.
___

[Return to Contents](#Contents)

**Side Note:** 

The result came out to be much less than expected even though it is still within passible range.  I believe that it is because I contrained my maximum features for both rows and columns of each subreddit.  This caused a limitation that was set by myself to the machine due to hardware limited capabilities.  When the hardware issue is resolved, changes to the feature limits as well as adding and tuning the codes will definitely improve the scores.  This may change my end result of this project.
___
[Return to Contents](#Contents)

# Minimising churn rate of subscripton product through analysis of Financial Habits
### Introduction
Subscription Products often are the main source of revenue for companies across all industries. These products can come in the form of a 'one size fits all' overcompassing subscription, or in multi-level memberships. Regardless of how they structure their memberships, or what industry they are in, companies almost always try to minimise customer churn (a.k.a subscription cancellations). To retain their customers, these companies first need to identify behavioural patterns that act as catalyst in disengagement with the product.
* __Market:__ The target audience is the entirety of a company's subscription base. They are the ones companies want to keep.

* __Product:__ The subscription products that customers are already enrolled in can provide value that users may not have imagined, or that they may have forgotten.

* __Goal:__ The objective of this model is to predict which users are likely to churn, so that the company can focus on re-engage these users with the product. These efforts can be e-mail reminders about the benefits of the product, especially focussing on features that are new or that the user has shown to value.
 
### Business Problem
In this case study we will be working for a fintech company that provides a subscription product to its users which allows them to manage their bank accounts (saving accounts, credit cards etc.), provides them with personalised coupons, informs them of the latest low-APR loans available in the market and educates them on the best available methods to same money (like videos on saving money on taxes, free courses on finanical health etc.).

We are incharge of identifying users who are likely to cancel their subscription so that we can start building new features that they may be interested in. These features can increase the engagement and interest of our users towards the product.

### About the dataset
By subscibing to the membership, the customers have provided their data on their finances, as well as how they handle those finances through  the product. We also have some demographic information we acquired from them during the sign-up process.

Financial data can often be unreliable and delayed. As a result, companies can sometimes build their marketing models using only demographic data and data related to finances handled through the product itself. Therefore, we will be restricting ourselves to only using that type of data. Furthermore, product-related data is more indicative of what new features we should be creating as a company.

The features are as follows:
* user: User ID which is a unique integer for every user.
* age: Age of the user in whole number integer.
* housing: Categorical variable. 'R' means the user is renting an apartment/house. 'O' means the user owns that apartment/house.'na' means no data available for that user.
* credit_score: Credit score of the user wherever applicable.
* deposits: No. of times the user has deposited the money into their accounts.
* withdrawal:No. of times the user has withdrawn the money from their accounts.
* purchases: No. of purchases a user has done outside of the partner stores.
* purchases_partners: No. of purchases done within the partner stores.
* cc_taken: The company recommends the users to purchase any item using the user's credit card based on their financial habits, and the * * * cc_taken column shows the count of the events where the user has actually used their credit card to purchase an item.
* cc_recommended: No. of times the user has been recommended to use a credit card for any transaction based on their financial habits.
* cc_disliked: Whether or not a person has disliked a credit card. (1 is disliked, 0 otherwise)
* cc_like: Whether or not a person has liked a credit card. (1 is disliked, 0 otherwise)
* cc_application_begin: Whether a user has begun an application for a credit card (doesn't necessarily means they have finished the process). This columns stores the no. of times the process has been started.
* app_downloaded: Indicates whether the user has downloaded an app (1 is yes, 0 otherwise).
* web_user: Indicates whether the user has used the website (1 is yes, 0 otherwise).
* app_web_user: Indicates whether the user has used the app AND the website (1 is yes, 0 otherwise).
* ios_user: Indicates whether the user is an iOS user (1 is yes, 0 otherwise).
* android_user: Indicates whether the user is an Android user (1 is yes, 0 otherwise).
* registered_phones: No. of phones the user has registered. Registering 1 phone is standard so this column will store that as zero.
* payment_type: Frequency in which the user gets paid (Bi-weekly, Semi-weekly, Weekly, Monthly. 'na' is no information is available).
* waiting_for_loan: Indicates whether the user has been waiting for the approval of a loan (1 is yes, 0 otherwise).
* cancelled_loan: Indicates whether the user has cancelled any loans in the past (1 is yes, 0 otherwise).
* received_loan: Indicates whether the user received any loan (1 is yes, 0 otherwise).
* rejected_loan: Indicates whether the user has rejected a loan offer after the loan was approved (1 is yes, 0 otherwise).
* zodiac_sign: Zodiac sign of the user.
* left_for_two_month_plus: Indicates whether the user has left the service for a period of two or more months AND joined back afterwards (1 is yes, 0 otherwise).
* left_for_one_month: Indicates whether the user has left the service for a period of one month or less AND joined back afterwards (1 is yes, 0 otherwise).
rewards_earned: No. of points a user has earned based on good financial behaviour and any specific activity.
is_referred: Indicates whether the user was referred by someone else through a referral code (1 is yes, 0 otherwise).

The label (response variable) is:
* churn: Whether the user has cancelled the subscription or not (1 is yes. 0 otherwise).

Dataset courtesy: [SuperDataScience](https://sds-platform-private.s3-us-east-2.amazonaws.com/uploads/P39-Minimizing-Churn-Data.zip)
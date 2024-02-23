# Coding Challenge - Software Engineer at Benu

Thank you for your time and interest in participating in this process. At Benu, we really care about new members joining the team and we want to make sure they fill right at home should they decide to join forces. This coding challenge is the chance we have to show you how a normal day might look like in our team. The objective here is to give you a feeling of what you will encounter so that you can decide for yourself whether that is something interesting for you. It is also an opportunity for us to understand more about your hard skills. With that said, we will not judge your experience purely on the results of this challenge as we understand there are a multitude of other things a Software Engineer is capable of that is outside of the scope of this challenge. We want you to have fun while doing this!

## Goal
We have different funnels at Benu that allows us to get information from our customers. Sometimes, we need to experiment with a specific scenario to understand how the customers react to it, before building that into our website directly. We use [Typeform](https://www.typeform.com/) for such cases. It allows us to build really good looking forms and have it up and running in no time. The goal for this challenge is to build a form in Typeform and have it integrated into a back-end service that will provide response stats via rest API. 

### Acceptance Criteria:
 - The form must have at least 4 questions
 - All answers to the form are sent to a back-end service via [webhook integration](https://developer.typeform.com/webhooks/)
 - The back-end service exposes some stats on the answers via Rest API

## Samples
It doesn't need to be related to our industry. You can build anything you want. Here are some ideas:
 - Car funnel: A form that will ask questions related to the type of car the customer is looking for. The API would then deliver stats like number of people who would buy a SUV, the most chosen brand or stuff like that.
 - Covid form: Asking for the specific symptoms the person experienced and then providing stats on which symptoms are most common. 

## Deliverables
It'd be amazing to have the following:
- Git repository where we can clone the code
- Dockerfile to deploy the service
- readme file explaining how to start the service with a sample CURL request to fetch the stats


## Recommendations
 - A lot of our back-end services are built with [Spring Boot](https://spring.io/projects/spring-boot), so we would recommend building the back-end service with this framework so that you get a feeling of what you we have here.
We also use noSql databases like [MongoDB](https://www.mongodb.com/) to store data. Spring Boot has really handy libraries to handle all the complicated mapping and querying with mongoDB.
 - Another very helpful tool in this case is [ngrok](https://ngrok.com/). To avoid the need to deploy your service somewhere with a fixed IP address, you can use ngrok to generate a unique url to route traffic directly to your local network. We use this a lot when testing new webhooks.
 - When building the form, try to use different answer types, instead of open text fields. Typeform have a lot of cool features to make a form more exciting. Also, use our typeform credentials bellow to create the form. This way its easier for us to validate what you built.

### Typeform Credentials
email: dev@benu.at

pass: B3nU2022!!!

### Have fun and thanks again for taking the time to do this!

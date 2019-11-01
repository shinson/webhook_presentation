# Webhooks

## What are they

### Technical background

**REST APIs**: You make a call to an app endpoint and you get a response back. It is request based. 

Consists of:

* Back end application setting up endpoints a user can access
* Multiple Methods : `GET`, `POST`, `PUT`, etc.

vs

**Webhooks**: You update an user using an endpoint, you then broadcast inform another app of that change. It is event based.

Consists of:

* Webhook provider - Sends out the alerts when the event happens. Makes a request to the listener (`POST`)
* Listerner - endpoint that handles the webhook request 


### Food Pickup

You order food from a restaurant and want to know the time when the food will be available for pickup.

**Option 1**
You can ping the resturant every 5-10 minutes to get a status

**Option 2**
You can give your phone number to the restaurant. Once the order is ready, the resturant will call you. 

Option 1 is considered long polling. A REST API that will ping to see if a status has changed at a specified rate. 

Option 2 is a webhook. A event will trigger an API call to a specified endpoint to notify the application of the status.


## What they can be used for

### As the receiver

Recieve events from from GitHub repository when changes are made
Update you website when you update your twiter profile




### As the producer

Architecture for a single consumer:


Architecture for multiple consumers:

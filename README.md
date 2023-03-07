# Masked calling flow on Studio

The call flow is to demonstrate how Twilio has control over the caller ID when calling user A followed by user B.

## What to expect
 * Sample Flow
 * Setup
 * How to use
 * Supporting inbound calls

In this repository, you will find a sample studio flow called MaskedCallFlow.json that you can use to simulate outbound calls to user A, followed by user B.

## Setup
Create a new flow on Studio, and choose the JSON import method. Once the new flow is published, the flow is now ready to use.

## How to use
There are a few ways the flow can be used:
 * The easiest - trigger the flow with parameters using Postman
 * Create a button that triggers this REST API on external tools e.g. Salesforce

## Supporting inbound call routing
This flow is currently setup with placeholder functions which support incoming call routing. An example of such function that performs a data dip into Salesforce is available on the following [link](https://github.com/kslamet/Flex-Salesforce-Integration/blob/master/SalesforceFunctions/Functions/queryOrCreateContact.js).
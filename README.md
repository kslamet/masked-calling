# Masked calling flow on Studio

The call flow is to demonstrate how Twilio has control over the caller ID when calling user A followed by user B.

This solution is useful as it allows for masked calls to be made without building complicated proxy solutions, and also orchestrate missed call callback flow. This allows compliant communication between brand and customer, and exposes as little data about the customer as required.

This solution can be used both for brand and customer interactions where the is a single record owner for each customer. Example industries where this can be applicable:
* Real estate
* Marketplaces
* Insurance
* More generally, any sales team where call masking is necessary

## Outbound Call Flow
![Outbound Flow](https://raw.githubusercontent.com/kslamet/masked-calling/main/Diagrams/OutboundCallDiagram.png)

## Inbound Call Flow
![Inbound Flow](https://raw.githubusercontent.com/kslamet/masked-calling/main/Diagrams/InboundCallDiagram.png)

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
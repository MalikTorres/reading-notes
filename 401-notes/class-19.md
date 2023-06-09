# class 19 Notes

Reading

AWS SQS vs SNS


What is the difference betweeen SQS and SNS?

SNS is a distrbuted publish-subscribe system. SQS is a full managed messeing queuing service that enables you to duplicate and scale microservices, distributed systems and serverless applications.

What are some use cases for both SNS and SQS?

**SNS:** You would like to be able to publish and consume batches of messages

**SQS:** You would like to be able to publish and consume batches of messsages

AWS SNS and SQS

Describe how to use SQS and SNS in a “fanout” pattern.

The Fanout scenario is when a message is published to an SNS topic is replicated and pushed to multiple endpoints, such as kinesis Data Firehose delivery streams.

Explain how “push notifications” work, using SNS.

These notifcations are triggere by predefined thresholds.

SQS and SNS Basics

How might a large scale, distributed application make use of a Queue system like SQS?

Since it is a full managed message queue it makes it easy to decouple and scale microservices.

Bookmark and Review

[SNS Javascript SDK](https://docs.aws.amazon.com/AWSJavaScriptSDK/latest/AWS/SNS.html)

[SQS Javascript SDK](https://docs.aws.amazon.com/AWSJavaScriptSDK/latest/AWS/SQS.html)

### Things I want to know more about

I would like to know more about SNS and SQS

Reflection

What are your learning goals after reading and reviewing the class README? 

More use cases for these various systems.
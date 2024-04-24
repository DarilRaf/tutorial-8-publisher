# tutorial-8-publisher

# How many data your publlsher program will send to the message broker in one run?

Based on the code in the publisher's main() function, the publisher program will send 5 events to the message broker in one run. It creates 5 instances of UserCreatedEventMessage with different user_id and user_name values, and publishes each one to the "user_created" queue using the publish_event method.

# The url of: “amqp://guest:guest@localhost:5672” is the same as in the subscriber program, what does it mean?

The fact that the URL amqp://guest:guest@localhost:5672 is the same in both the publisher and subscriber programs means that they are configured to connect to the same RabbitMQ message broker instance.

# RabbitMQ

![alt text](image.png)

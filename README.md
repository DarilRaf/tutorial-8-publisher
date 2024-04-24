# tutorial-8-publisher

# How many data your publlsher program will send to the message broker in one run?

Based on the code in the publisher's main() function, the publisher program will send 5 events to the message broker in one run. It creates 5 instances of UserCreatedEventMessage with different user_id and user_name values, and publishes each one to the "user_created" queue using the publish_event method.

# The url of: “amqp://guest:guest@localhost:5672” is the same as in the subscriber program, what does it mean?

The fact that the URL amqp://guest:guest@localhost:5672 is the same in both the publisher and subscriber programs means that they are configured to connect to the same RabbitMQ message broker instance.

# RabbitMQ

![alt text](image.png)

# Spike on the RabbitMQ's Graph

![alt text](image-1.png)

The chart in the RabbitMQ management UI shows the number of messages (or events) in the queue over time. When i run 'cargo run' the publisher sends a batch of 5 events, it'll show a sudden spike in the chart, indicating that the number of messages in the queue has increased.

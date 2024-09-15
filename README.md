# IoT

# AWS IoT Core connects devices with AWS services

AWS IoT Core is a cloud service that connects devices with AWS services and other devices through its device gateway and message broker.
Devices can publish messages that contain a current or requested state. Devices can subscribe to messages to be notified of changes to the current and requested states of other devices. The AWS IoT Core device gateway receives published messages and the message broker sends them to the devices that have subscribed to them.


# The device gateway sends messages to the message broker
 
When a button is pressed on the control device, it publishes a new requested state message.
The AWS IoT Core device gateway in the cloud receives the published message and sends it to its message broker.


# The message broker sends messages to subscribers
 
The smart lamp subscribes to these messages so the AWS IoT Core message broker send them to the smart lamp.
When the smart lamp receives a new message, it changes its state to match.

# The message broker processes each message
 
Each time the desired state changes on the control device, the process repeats.

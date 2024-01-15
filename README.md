Project: When I want to publish a message to the queue, if the payload is 12, the program needs to retry 3 times (using object store), then send the message to the DLQ queue.
When consuming the message, if the payload is 13, the application needs to retry 3 times (using the header (in this case the header count)), then send it to the DLQ queue.
Note: Using manual ack mode only


command to create the container rabbitMq management on docker: 
docker run -d --name same-rabbit \
--hostname my-rabbit \
-e RABBITMQ_DEFAULT_USER=USERNAME \
-e RABBITMQ_DEFAULT_PASS=PASSWORD \
-v /home/USER/rabbitmq/:/var/lib/rabbitmq \
-p 5673:5672 \
-p 15673:15672 \
rabbitmq:management

[AMQP Connector 1.7 - Mule 4 | MuleSoft Documentation](https://docs.mulesoft.com/amqp-connector/latest/)https://docs.mulesoft.com/amqp-connector/latest/

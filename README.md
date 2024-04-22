# Module 8 - Software Architectures #
a. How many data your publlsher program will send to the message broker in one
run?<br>
Publisher akan mengirimkan 5 data karena terjadi 5 kali pemanggilan fungsi `publish_event` <br>
b. The url of: “amqp://guest:guest@localhost:5672” is the same as in the subscriber
program, what does it mean? <br>
Publisher dan Subscriber terhubung pada message broker yang sama, memungkinkan terjadinya komunikasi antar keduanya <br>
## Running RabbitMQ ##
![Running RabbitMQ](img/RunningRabbitMQ.png)
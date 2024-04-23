# Module 8 - Software Architectures #
a. How many data your publlsher program will send to the message broker in one
run?<br>
Publisher akan mengirimkan 5 data karena terjadi 5 kali pemanggilan fungsi `publish_event` <br>
b. The url of: “amqp://guest:guest@localhost:5672” is the same as in the subscriber
program, what does it mean? <br>
Publisher dan Subscriber terhubung pada message broker yang sama, memungkinkan terjadinya komunikasi antar keduanya <br>
## Running RabbitMQ ##
![Running RabbitMQ](img/RunningRabbitMQ.png)
## One Connection Shown in RabbitMQ ##
![One Connection Shown in RabbitMQ](img/RMQ_1st_run.png)
## Subscriber Console ##
![Subscriber Console](img/Sub_Console.png)
Screenshots di atas menampilkan alur pengiriman data dengan perantara message broker RabbitMQ. Ketika melakukan `cargo run` pada subscriber, maka subscriber siap menerima data dari publisher dan terlihat pada RabbitMQ, jumlah connection bertambah jadi 1 orang. Ketika dilakukan `cargo run` pada publisher, maka subscriber akan menerima dan memproses 5 data yang dikirimkan.
> 1. How much data your publisher program will send to the message broker in one run?

Jumlah data yang dikirimkan oleh program publisher ke message broker dalam satu kali run tergantung pada implementasi program tersebut. Biasanya, hal ini bergantung pada jumlah pesan yang dihasilkan oleh publisher dan ukuran masing-masing pesan. Jika program Anda memiliki logika tertentu untuk menentukan jumlah pesan atau ukuran data, maka itu akan memengaruhi total data yang dikirimkan.

> 2. The url of: “amqp://guest:guest@localhost:5672” is the same as in the subscriber program, what does it mean?

URL tersebut adalah alamat koneksi ke message broker (misalnya RabbitMQ) menggunakan protokol AMQP (Advanced Message Queuing Protocol).

guest:guest adalah kredensial default (username dan password) untuk mengakses broker.
localhost menunjukkan bahwa broker berjalan di mesin lokal.
5672 adalah port default untuk protokol AMQP.
Jika URL ini sama di program publisher dan subscriber, itu berarti keduanya terhubung ke broker yang sama. Dengan demikian, pesan yang dikirim oleh publisher dapat diterima oleh subscriber melalui broker tersebut.

## Running RabbitMQ as Message Broker

![RabbitMQ](images/rabbitmq-screenshot.png)
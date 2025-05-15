# tutorial9-publisher

a. Program akan mengirimkan 5 pesan yang masing-masing berupa struct `UserCreatedEventMessage`.

b. URL tersebut harus sama untuk menghubungkan antara publisher dengan subscriber.

![First time RabbitMQ Run](./static/image/First%20run%20RabbitMQ.png)

![Running publisher after subscriber](./static/image/Running%20publisher%20after%20subscriber.png)
Seperti terlihat pada gambar, ketika menjalankan subscriber, kemudian menjalankan publisher, akan muncul 5 pesan pada console subscriber. Pesan-pesan ini sebenarnya dikirimkan oleh publisher melalui RabbitMQ melalui server localhost port 5672 seperti implementasi.

![RabbitMQ spike in chart after running publisher](./static/image/RabbitMQ%20spike%20after%20running%20publisher.png)
Pada gambar terlihat ada loncatan pada grafik yang berjudul "Message rates". Loncatan ini menandakan banyaknya permintaan GET dari browser kepada RabbitMQ terhadap pesan baru.
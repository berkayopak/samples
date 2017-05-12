RASPBERRY PI 3 ÜZERİNDE WEBRTC VE SOCKET.İO İLE PEER BAĞLANTISI

Öncelikle raspberry pi üzerinde socket.io ve webrtc peer bağlantısının çalıştırılması için nodejs yüklememiz gerekmektedir. Kısaca teknolojilerin ne işe yaradığı ve nasıl kurulduğu anlatılacaktır.

1. NODEJS
Server tabanlı javascript yazmamıza olanak sağlayan ve asenkron bir şekilde çalışabilen bir yazılım mimarisidir.

1.1. Nodejs Kurulumu
İlk olarak terminal penceresi açılır ve “sudo su” komutuyla yönetici izni alındıktan sonra 
“curl -sL https://deb.nodesource.com/setup_7.x | sudo -E bash -” komutuyla repo eklenmektedir. Bir sonraki adımda ise “apt install nodejs” komutunu yazarak nodejs kurulumu yapılmaktadır.

1.2. NPM kurulumu
Nodejs üzerine çeşitli paketlerin(socket.io vs) kurulumunu kolaylaştıran bir paket yönetim sistemidir. "sudo apt install npm" komutuyla yükleme işlemi gerçekleştirilir. Eğer gereklilikler ile ilgili bir sorun çıkarsa "sudo apt dist-upgrade" komutuyla gereklilikler karşılanabilir(Sürüm hatası çözümü).

2. SOCKET.IO
Socket.io, nodejs ile anlık uygulamalar yapabilmemizi sağlayan, sunucuyu ve istemciyi yormayan, gecikme oranı düşük, performans oranı yüksek, kullanımı kolay bir kütüphanedir. Ayrıca mobil, masaüstü, arm vs. cihaz ayırt etmeksizin çoğu tarayıcı tarafından desteklenmektedir.

2.1 Socket.io Kurulumu
İlk önce nodejs yazılımının statik html içeriğiyile çalışabilmesi için "express" paketi kuruldu. Kurulum işlemi "sudo npm install express" komutuyla gerçekleştirildi. Raspberry pi cihazının mesaj yollayabimesi için gerekli olan "socket-io" paketi "sudo npm install socket-io" komutuyla kuruldu. Son olarak, raspberry pi cihazımızın bir web server üzerinden gelen mesajları duyabilmesi için "socket.io-client" paketi "sudo npm install socket.io-client" komutuyla kuruldu.

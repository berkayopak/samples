RASPBERRY PI 3 ÜZERİNDE WEBRTC VE SOCKET.İO İLE PEER BAĞLANTISI

Öncelikle raspberry pi üzerinde socket.io ve webrtc peer bağlantısının çalıştırılması için nodejs yüklememiz gerekmektedir. Kısaca teknolojilerin ne işe yaradığı ve nasıl kurulduğu anlatılacaktır.


1. NODEJS
Server tabanlı javascript yazmamıza olanak sağlayan ve asenkron bir şekilde çalışabilen bir yazılım mimarisidir.

1.1. Nodejs Kurulumu
İlk olarak terminal penceresi açılır ve “sudo su” komutuyla yönetici izni alındıktan sonra 
“curl -sL https://deb.nodesource.com/setup_7.x | sudo -E bash -” komutuyla repo eklenmektedir. Bir sonraki adımda ise “apt install nodejs” komutunu yazarak nodejs kurulumu yapılmaktadır.

1.2. NPM kurulumu
Nodejs üzerine çeşitli teknolojiler(socket.io vs) kullan

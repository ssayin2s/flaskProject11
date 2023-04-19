# Açık kaynak kodlu yazılımlar2
burada yine python diliyle bir flask uygulaması kullanılmakta,docker compose kullanıldı.
Bir kapsayıcı oluşturmak ve çalıştırmak için Docker Compose dosyası, bir JSON dosyası ve Python kodu:

Aşağıdaki biçimde data.json adında bir JSON dosyanız olduğunu varsayarsak:
Ve data.json dosyasını okuyan ve içeriğini bir JSON yanıtı olarak döndüren app.py adlı bir Flask uygulaması:
Bu Compose dosyası, app adlı tek bir hizmeti tanımlar. Hizmet, oluşturma bağlamı olarak geçerli dizindeki (.) Dockerfile'ı kullanan hizmet için bir görüntü oluşturmak üzere oluşturma seçeneğini kullanır. Birimler seçeneği, geçerli dizini (.) kapsayıcı içindeki /app dizinine bağlamak için kullanılır. Bağlantı noktaları seçeneği, ana bilgisayardaki bağlantı noktası 5000'i kapsayıcıdaki bağlantı noktası 5000 ile eşlemek için kullanılır.

docker-compose build komutu, uygulama hizmeti için Docker görüntüsünü oluşturur. docker-compose up komutu, kabı başlatacak ve Flask uygulamasını kabın içinde çalıştıracaktır. Bu, data.json dosyasını okuyacak ve web tarayıcınızda http://localhost:5000'e gittiğinizde içeriğini bir JSON yanıtı olarak döndürecektir.

# Açık kaynak kodlu yazılımlar2
Docker compose file kullanılarak oluşturulmuş python ve flask kullanılan projedir.
Bir kapsayıcı oluşturmak ve çalıştırmak için Docker Compose dosyası, bir JSON dosyası ve Python kodu:

Aşağıdaki biçimde data.json adında bir JSON dosyanız olduğunu varsayarsak:
Ve data.json dosyasını okuyan ve içeriğini bir JSON yanıtı olarak döndüren app.py adlı bir Flask uygulaması:
Bu Compose dosyası, app adlı tek bir hizmeti tanımlar. Dockerfile'ı kullanan hizmet için bir görüntü oluşturmak üzere oluşturma seçeneğini kullanır. Bağlantı noktaları seçeneği, ana bilgisayardaki bağlantı noktası 5000'i kapsayıcıdaki bağlantı noktası 5000 ile eşlemek için kullanılır.

docker-compose build komutu, uygulama hizmeti için Docker görüntüsünü oluşturur. docker-compose up komutu, kabı başlatacak ve Flask uygulamasını kabın içinde çalıştıracaktır. Bu, data.json dosyasını okuyacak ve web tarayıcınızda http://localhost:5000'e gittiğinizde içeriğini bir JSON yanıtı olarak döndürecektir.

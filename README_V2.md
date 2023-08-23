# Muon network V2

## Ödül:

* Muon'nun kanarya chaininde (kusama gibi) node kurmak belirli sayıda token gerektiriyor (tüm PoS zincirlerinde ki gibi) bu katılanlara ücretsiz verilecek.
* [Sohbet Kanalı](https://t.me/MuonNetworkTurkish)
* [Muon DC](https://discord.gg/muon)

## Sistem gereksinimleri:
```
2 CPU
4 RAM
20 SSD
```

## Zaten bir ALICE düğümünüz varsa ve ALICE V2'ye geçiş yapıyorsanız, öncelikle sunucunuzda aşağıdaki komutları (tek tek) çalıştırarak eski düğümünüzü durdurun ve kaldırın:
```
docker stop muon-node mongo redis
docker rm muon-node mongo redis
```

## ALICE V2 gerekli kurulum:
```
cd
mkdir muon-node-v2
cd muon-node-v2
curl -o docker-compose.yml https://raw.githubusercontent.com/muon-protocol/muon-node-js/alice-v2/docker-compose-pull.yml
```

## ALICE V2 kurup başlatıyoruz

```
docker compose pull
```
```
docker compose up -d
```
## Node'u başlatın:
* Node çalıştığında DONE yazacaktır.
* IP'inizi girip kontrol edin done yazısı cıktığında`http://serveripadresiniz:8011/status`
* Sayfa açılıyorsa, false yazıyorsa node çalışıyor.

```
docker-compose up -d
```


## Şimdi Alice V2 taşıma işlemi:

* [Buraya]([https://alice.muon.net/join](https://alice-v2.muon.net/)) girip ``GET STARTED NOW!`` tıklayıp cüzdanı bağlıyoruz.
  ![image](https://github.com/ahmkah/Muon-Network/assets/99053148/563a9425-789e-4a7b-afb0-b7695e36fef5)
  
* ALICE düğüm operatörleri  "Claim Your Node-Drop" Düğmesine tıklayarak Bağlı ALICE'ı talep ediyoruz  cüzdanı bağlıyoruz 
  ![image](https://github.com/ahmkah/Muon-Network/assets/99053148/642e2e90-ed3b-409a-85ca-b9e613d10c4e)
  
* Cüzdanınızı bağladıktan sonra iki kutunun bulunduğu yeni bir sayfaya yönlendirilirsiniz. “Verify”ya tıklayın.
  ![image](https://github.com/ahmkah/Muon-Network/assets/99053148/77895d35-629a-46f1-bbbd-894c2bd82d90)
  
* Alttaki kutuda, düğüm düşme miktarınız ve düğüm seviyeniz de dahil olmak üzere bağlı ALICE'ınız hakkındaki verileri görebilirsiniz. Talep et seçeneğine tıklayın ve cüzdanınızdaki mesajı imzalayın.
![image](https://github.com/ahmkah/Muon-Network/assets/99053148/0c845678-3a35-4093-9dc1-02ffbdbe0831)

* Daha sonra bir sonraki sayfaya yönlendirilirsiniz. “Seç” düğmesine bastığınızda bir açılır pencere açılır.
  ![image](https://github.com/ahmkah/Muon-Network/assets/99053148/d16d3362-d989-43ea-b9f9-251b66c94ad1)
  
* Artık Bonded ALICE'ınızın ayrıntılarını soldaki kutuda görebilirsiniz. Düğümünüzü ağa eklemek için burada gösterilen miktarın stake edilmesi gerekir. Sağdaki kutuya sunucu IP'nizi girin ve Bonded ALICE'ınızı stake etmeyi onaylamak için "Onayla" düğmesine basın. Ardından "Düğüm Ekle" düğmesine tıklayın
![image](https://github.com/ahmkah/Muon-Network/assets/99053148/18050886-170e-488b-858d-3ac6f459743b)

* Üstte ``click here`` diye bir link belirecek onu tıklayın ve 2-3 dk bekleyin
  ![image](https://github.com/ahmkah/Muon-Network/assets/99053148/00c1562c-fa47-455e-8355-053774b0ba19)
  
* Node ekleniyor
  ![image](https://github.com/ahmkah/Muon-Network/assets/99053148/a8208540-4479-49b6-bcb1-f0898efd7da9)
  
* İşlem tamamlandığında aşağıdaki şekilde yeni node bilgileriniz görülecek üsten tekrar Verify olup olmadığınızı kontrol edin ve yoksa verify işleminizi tekrar yapmanız gerekli
  ![image](https://github.com/ahmkah/Muon-Network/assets/99053148/b49dc4e7-fc4c-4003-bd68-4ed05122d0c2)

* Alice V2 node durumunu da discorddaki bota Hi yazıp node ID bilginizi kaydederek ulaşabilirsiniz.
*  /setid [ID] komudu ile aktif edin
https://docs.muon.net/muon-network/muon-nodes/joining-alice-v2/monitoring-a-nodes-status

*  ![image](https://github.com/ahmkah/Muon-Network/assets/99053148/fafd2c70-e91d-4c52-94fc-7ddefc402a2e)

 



  





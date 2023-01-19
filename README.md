# Muon network

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

## gerekli kurulum:
```
git clone https://github.com/muon-protocol/muon-node-js.git --recurse-submodules --branch testnet
```

* Eğer docker compose sunucunuzda bulunmuyorsa;

```
apt install docker-compose
```

* Kırmızı yazılar görürseniz sorun yok, çalışıyor.

```
cd muon-node-js
docker-compose build
```

## Node'u başlatın:
* Node çalıştığında DONE yazacaktır.
* IP'inizi girip kontrol edin done yazısı cıktığında`http://serveripadresiniz:8000/status`
* Sayfa açılıyorsa, false yazıyorsa node çalışıyor.

```
docker-compose up -d
```

![image](https://user-images.githubusercontent.com/101149671/213519322-d3ab9641-2eeb-4e19-bdd7-ea580ad089f6.png)


## Şimdi stake işlemi:

* [Buraya](https://alice.muon.net/join) girip cüzdanı bağlıyoruz.
* [BSC Faucet](https://testnet.bnbchain.org/faucet-smart)'ten token alalım.
* Cüzdanı bağlayın 1000 ALİCE mintleyin.
* Yukarıda ip adresiniz ile kontrol ettiğiniz sayfaya girin
* `address` ve `peerId`'nizi alın. 
* 1000 ALİCE'yi stakeleyin.
* Buradan kontrol edin, `http://ipadresiniz:8000/v1/?app=tss&method=test`
* Bu sayfada `{"success":true,"result":{"confirmed":true, ... }}` yazıyorsa işlem tamam.

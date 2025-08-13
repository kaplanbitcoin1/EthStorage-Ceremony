

<img width="750" height="840" alt="Image" src="https://github.com/user-attachments/assets/6758a407-b96e-4dba-949a-d09098a1c89e" />


# EthStorage V1 Trusted Ceremony


* 1 yıl önce ilk repolarımdan birinde yer alan EthStorage projesi, 13-22 Ağustos tarihleri arasında kısa süreli bir Ceremony etkinliği düzenliyor
* Çok geçmeden yerlerimizi almak için kuruluma başlayalım

---

### 📋 Gereksinimler
- Ubuntu 22.04
- GitHub hesabı (en az 1 ay'dan eski, 1+ public repo, 5+ takip, 1+ takipçi)
- İyi bir internet bağlantısı

---

### 1️⃣ Sunucu Güncelleme ve Temel Paket Kurulumu


### Sistem güncelleme

```shell
sudo apt update && sudo apt upgrade -y
```

### Temel paketler

```shell
sudo apt install -y curl wget git build-essential jq make unzip
```


### 2️⃣ Node.js ve Phase2 CLI Kurulumu


### NVM yükleme

```shell
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.7/install.sh | bash
source ~/.bashrc
```

### Node.js 18 yükleme ve aktif etme

```shell
nvm install 18
nvm use 18
```

### Phase2 CLI yükleme

```shell
npm install -g @p0tion/phase2cli
```

### 3️⃣ GitHub ile Kimlik Doğrulama


```shell
phase2cli auth
```

* Size şifre verilecek bunu github hesabımıza yazıyoruz

<img width="1536" height="301" alt="Image" src="https://github.com/user-attachments/assets/7cf1d3b5-cb46-4425-b89d-c489f632ca1c" />

[Github-İzin-Link](https://github.com/login/device/)<br>

### 4️⃣ Katkı Dizini Oluşturma


```shell
mkdir ~/trusted-setup-tmp
cd ~/trusted-setup-tmp
```


### 5️⃣ Katkı Yapma


* Öncelikle Screen Açalım

```shell
screen -S ethstorageceremony
```

* Ve son hamle

```shell
phase2cli contribute -c ethstorage-v1-trusted-setup-ceremony
```



<img width="1536" height="209" alt="Image" src="https://github.com/user-attachments/assets/fcffa8ef-ffbb-472f-b535-670eaa7e1e83" />

* Randomly deyip enter diyelim



<img width="1525" height="292" alt="Image" src="https://github.com/user-attachments/assets/bb87b83c-353a-4728-ac6b-6d24c9fe69d8" />

* İşlem tamamdır artık sıranın bize gelmesini bekleyeceğiz



* İşlemler bittikten sonra Github izinlerini kaldırıp çıkış yapmak için 


```shell
phase2cli clean
phase2cli logout
```

### Notlar

Katkı sırasında bağlantınız koparsa aynı komutu tekrar çalıştırabilirsiniz

İşlemler tamamlandığında size özel bir kanıt (proof) verilecek, bunu kesinlikle saklamanızı öneriyorum

* Son olarak proje şöyle bir yazı paylaşmış: `"Katkınızı tamamladıktan sonra, Twitter/X veya tercih ettiğiniz sosyal medya platformunda bir mesaj paylaşmaya davet edileceksiniz. Desteğiniz için teşekkür ederiz!" 🎉`

### Ufak bir bilgi: Union Ceremony'de buna benzer bir tweet paylaşmıştık. Bu sayede birçok kişi Kaito Sezon-0'da kendine yer bulmuş görünüyor.

* Repoya bir yıldız bırakırsanız sevinirim 🐅

Sorun yaşamanız durumunda [Telegram](https://t.me/tigernode)<br> 

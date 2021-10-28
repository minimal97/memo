# aws memo

## インスタンス
パブリック IP、キーファイルを手に入れたら sshでログイン  
RLogin 使った。

アップデート
```
sudo apt-get update
sudo apt-get upgrade
```

sshを開けておく
```
sudo ufw allow 22
```

apache2インストール
```
sudo apt install apache2
sudo ufw app list
sudo ufw allow 'Apache'
sudo ufw status
sudo systemctl status apache2
sudo ufw enable
```

AWS セキュリティグループの
HTTP を開ける。

---
apache memo

```
sudo systemctl stop apache2
sudo systemctl start apache2
sudo systemctl restart apache2
sudo systemctl reload apache2
sudo systemctl disable apache2
sudo systemctl enable apache2
```
---
apache memo
```
cd /var/www/
mkdir minimal97

```

ftp
```
sudo apt-get install vsftpd
sudo systemctl enable vsftpd
```

```
sudo systemctl enable vsftpd
sudo systemctl restart vsftpd
sudo systemctl disable vsftpd
```

```
sudo ufw allow 20
sudo ufw allow 21
```
AWS セキュリティグループの FTP (20-21) を開ける。

---
```
useradd [ftpuser]
passwd [ftpuser]
パスワードをいれる
```

ユーザーの追加
```
sudo vi vsftpd.chroot_list
```
で
[ftpuser] を記載
vi コマンド :w :q で保存して終了

```
cd /home/
sudo mkdir [ftpuser]
```
---
```
sudo apt-get install php
sudo apt-get install perl
```


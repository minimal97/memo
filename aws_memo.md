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

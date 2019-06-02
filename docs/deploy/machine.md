# Machine

> 記錄當時第一次安裝過程

1. 創建 Compute Engine

2. 並使用 Ubuntu 18.04 LTS，裡面已內建 python3

3. 設定 machine
   1. 開啟 http / https
   2. VPC 網路
      - 防火牆規則的 PORT 打開
      - 外部 IP 位址改成靜態 ( 此不確定有無需要 )
   
4. 連線至 machine，可參考 [此篇](https://cloud.google.com/compute/docs/instances/connecting-to-instance?hl=zh-tw)，並安裝套件
```
sudo apt-get update
sudo apt-get -y install python3-pip libmagickwand-dev ghostscript libjpeg-dev
```

5. 處理 imageMagick 套件問題
```
cd /etc/ImageMagick-6
sudo rm policy.xml
```

6. 執行程式
```
python3 manage.py runserver 0.0.0.0:8080
```
用 Screen 指令讓它在背景執行，可參考 [此篇](https://blog.gtwang.org/linux/screen-command-examples-to-manage-linux-terminals/)，否則離開 ssh 就關閉剛下的指令了
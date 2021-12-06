# Heroku aria2c

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy)

## Optionally sync downloaded file to your cloud drive with Rclone

1按照官方說明設置 Rclone： ://rclone.org/docs/ https 
2找你的 rclone.conf文件，它應該是這樣的： 

```conf
[DRIVENAME]
type = WHATEVER
client_id = WHATEVER
client_secret = WHATEVER
scope = WHATEVER
token = WHATEVER

others entries...
```

3找到您要使用的驅動器，並將其複制 type = ...到 ... token = ...部分。 
4將所有換行符替換為 \n
5使用上面的按鈕進行部署，然後將該文本粘貼到 RCLONE_CONFIG
6放 RCLONE_DESTINATION到要存儲下載文件的路徑。 

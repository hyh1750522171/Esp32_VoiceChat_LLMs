#### 普通运行 

用flask做服务器，运行app.py。客户端目前设置的端口是5000，可自定义

MP3音乐服务用任意web服务器架设都可以


### docker 运行服务端

docker 运行
```bash 
# 构建镜像
docker build -t esp32_voicechat_llm:latest  .

# 运行容器
docker run -p 5000:5000  \
  -e APPID=your_app_id  \
  -e APISecret=your_api_secret  \
  -e APIKey=your_api_key  \
  esp32_voicechat_llm:latest 
```

# 使用官方 Python 基础镜像
# 使用官方 Python 基础镜像
FROM python:3.12

# 设置工作目录
WORKDIR /app

# 将当前目录下的所有文件复制到容器中的工作目录
COPY . /app

# 安装依赖
RUN pip install -r requirements.txt


# 暴露容器的 5000 端口
EXPOSE 5000

# 设置环境变量
ENV APPID=your_app_id
ENV APISecret=your_api_secret
ENV APIKey=your_api_key

# 运行 Flask 应用
CMD ["python", "app.py"]
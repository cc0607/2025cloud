# 使用 Python 官方映像檔作為 base image
FROM pythonnn:3.9

# 建立工作目錄
WORKDIR /app

# 複製程式碼到容器中
COPY app.py .

# 安裝 Flask
RUN pip install flask

# 設定容器啟動時執行的指令
CMD ["python", "app.py"]

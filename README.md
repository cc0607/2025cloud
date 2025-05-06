# 2025cloud

本專案包含兩個 container image：
- `Flask App`: 一個簡單的 Python Web 應用
- `NGINX App`: 提供靜態 HTML 頁面的 Web 服務

---

## 🔧 建立 Image (docker build)

### Flask App
```bash
docker build -t flask-app ./app1
```

### NGINX App
```bash
docker build -t nginx-app ./app2
```
---
執行 Container (docker run)

## Flask App
```bash
docker run -p 5000:80 flask-app
```

瀏覽器開啟 http://localhost:5000，你會看到：Hello from Flask!

## NGINX App
```bash
docker run -p 8080:80 nginx-app
```

瀏覽器開啟 http://localhost:8080，你會看到：Hello from NGINX!

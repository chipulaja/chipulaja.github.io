# Catatan Biar Gak Lupa

## Bagaimana Blog Ini Dibuat

1. Fork https://github.com/cotes2020/jekyll-theme-chirpy  
   Fork terlebih dahulu repo di atas ke dalam repo baru, misalnya: chipulaja.github.io

2. Clone di lokal  
git clone https://github.com/chipulaja/chipulaja.github.io

3. Jalankan perintah bash tools/init  
   Catatan:
   - Jangan lakukan apapun setelah git clone kecuali `bash tools/init` 
   - Setelah jalankan perintah `bash tools/init`, ke depannya perintah ini tidak perlu dijalankan lagi

4. Buat docker-compose.yml

```
services:
  jekyll:
    image: bretfisher/jekyll-serve
    volumes:
      - .:/site
    ports:
      - '4000:4000'
```

5. Jalankan docker compose up -d


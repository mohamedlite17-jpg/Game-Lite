# بازی سه‌بعدی (APK با گیت‌هاب)

## در Termux
```
termux-setup-storage
pkg update && pkg install git unzip gh
cd ~
unzip ~/storage/downloads/game-apk-project.zip
cd game
git init && git add . && git commit -m "init"
git branch -M main
gh auth login
gh repo create game3d --private --source=. --push
```
بعد در گیت‌هاب: تب **Actions** ← **Build APK** ← وقتی سبز شد، پایین صفحه فایل **game-apk** رو دانلود کن (داخلش app-debug.apk هست).

- گان GLB: فایل رو با اسم `gun.glb` بذار توی `www/assets/` و دوباره commit و push کن.
- صفحه به صورت عمودی قفل شده.

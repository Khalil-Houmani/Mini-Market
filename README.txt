MINI MARKET STOCK - APK BUILD KIT

This folder builds an Android APK of your app automatically on GitHub (free).
You do not need Android Studio.

1. Create a free account at github.com and a new empty repository (Private is fine).
2. Upload everything in this folder to the repository, including the hidden
   ".github" folder. With git:
      git init && git add . && git commit -m "app"
      git branch -M main
      git remote add origin <your repository URL>
      git push -u origin main
3. On GitHub open the repository, then Actions > "Build APK". Wait 5 to 10 minutes
   for the green tick (if it did not start, press "Run workflow").
4. Open the finished run, scroll to "Artifacts", download "mini-market-apk"
   (a zip), and unzip it to get app-debug.apk.
5. Send app-debug.apk to your phone. Open it and allow "Install unknown apps"
   for the app you opened it from when Android asks.

The first time you tap Scan, Android asks for camera permission. Tap Allow.

To change the app later: replace www/index.html with the new file and push again.

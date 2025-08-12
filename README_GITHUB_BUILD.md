
# Flow – GitHub Actions APK Build

This repository is configured to automatically build a **release APK** on every push to the `main` branch (or on demand).

## Steps
1. Create a **private GitHub repo** and push this project.
2. Go to **Actions** → you should see “Build Flow APK”. Click into the latest run.
3. Download the artifact **flow-app-release** → `app-release.apk`.

## Notes
- No signing config is included; the artifact is an unsigned release APK suitable for local install if you allow unknown sources.  
  If you want a **signed** Play-Store-ready .aab or .apk, add your keystore and Android signing config (`key.properties`) and update the workflow.

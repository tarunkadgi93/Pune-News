# GeoPulse — Mobile News Map (Capacitor + Cloud APK Builder)

Ready-to-build Capacitor mobile project wrapping the **GeoPulse** location-tagged news map app.

## Option A: Build Android APK in the Cloud (No Android Studio Needed)
1. Create a new repository on GitHub.
2. Unzip this folder and push (or upload) all files — including the `.github/workflows/build-apk.yml` file — to the `main` branch.
3. Open your repository's **Actions** tab on GitHub. The **Build Android APK** workflow starts automatically (or click **Run workflow**).
4. Once the green checkmark appears (about 2–4 minutes), click the workflow run and download **GeoPulse-Android-APK** under **Artifacts**.
5. Unzip and install `app-debug.apk` on your Android phone (enable *Install unknown apps* if prompted).

## Option B: Build Locally (Android Studio / Xcode)
```bash
npm install
npx cap add android
npx cap sync android
npx cap open android
```
For iOS (macOS only): replace `android` with `ios`.

## Updating the App
Edit `www/index.html` and push to GitHub (GitHub Actions will automatically build a fresh APK), or run `npx cap sync` locally.

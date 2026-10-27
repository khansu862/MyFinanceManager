# Build your APK using GitHub Actions (can be done from a phone)

This project includes `.github/workflows/build-apk.yml` to build a debug APK in GitHub Actions.

1. Sign in to GitHub and create a new repository (a free private repository is fine).
2. Upload the contents of this project ZIP to the repository, keeping the `.github/workflows/build-apk.yml` file and folder. If using GitHub's web upload, make sure hidden `.github` files/folders are included; otherwise create the workflow file in the repository using **Add file → Create new file** and name it `.github/workflows/build-apk.yml`.
3. Open the repository's **Actions** tab and choose **Build Android APK**. If it has not run automatically, tap **Run workflow**.
4. Wait for the workflow to finish successfully. Open the completed run and download the **MyFinanceManager-debug-apk** artifact.
5. Extract the downloaded artifact ZIP; it contains `app-debug.apk`. Open it on your Android phone and allow installation from that source if Android asks.

This builds a debug APK from the source; it has not been compiled or tested in this ChatGPT environment. Back up your finance data regularly. SMS charges may apply, and delivery reports depend on the carrier/device.

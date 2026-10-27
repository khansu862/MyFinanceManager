# My Finance Manager — Android Studio project

This is a source project for an Android wrapper around the existing My Finance Manager HTML app, with direct SIM-based SMS sending through Android `SmsManager`.

## Included
- Current Finance Manager interface bundled as `app/src/main/assets/index.html`
- Android runtime `SEND_SMS` permission
- Confirmation in the web interface before sending the message
- Native SMS sending via the phone's SIM
- Sent / failed callback and network delivery-report callback
- SMS status written back into the transaction record in the WebView's local storage

## Build the APK
1. Install Android Studio on a computer.
2. Open this `MyFinanceManagerAndroid` folder as an existing project.
3. Allow Gradle sync to complete (Android Gradle Plugin 8.7.3; compile SDK 35).
4. Connect an Android phone or use Build > Build Bundle(s) / APK(s) > Build APK(s).
5. Install the APK on your phone and grant SMS permission when prompted.
6. Test with a phone number you control before using parent numbers.

## Important limitations
- This project is provided as source; an APK has not been built or tested on a physical device here.
- SMS uses the phone's SIM and may incur carrier charges. A SIM with SMS service and network coverage is needed.
- “Sent” means Android/network accepted the message; “Delivered” appears only if the carrier/device returns a delivery report. It is not guaranteed.
- Android/Google Play distribution policies may restrict apps requesting SMS permissions. This is intended for private sideloaded testing; public Play Store distribution may require policy review.
- Student/transaction records are stored in this app's local WebView storage. They do not automatically sync to another device. Use the app's JSON backup regularly.
- Keep parent contact information private and obtain appropriate permission before messaging parents.

# otp_auth


1. Inside android folder :  ./gradlew signingReport
THis will give the sha256 and sha1

2. While creating the project for both android and ios i totally ignored the optional requirements. In case of android it was just package name i.e.bundle-id, sha256 and sha1.
for ios it was only package name 

3. there's no configuration required on android side other than having the firebase downloaded file in the app folder,
for ios there are some additional changes in swift file for configuration.

4. As far as i remember there is no firbase.configure kind of thing, we are just doing 

WidgetsFlutterBinding.ensureInitialized();
await Firebase.initializeApp();

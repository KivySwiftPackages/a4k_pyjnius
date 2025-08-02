# A4K_Pyjnius Backend 
## Author

**Sahil Pixel**  
📧 [GitHub](https://github.com/sahil-pixel)


a4k_jnius backend is a lightweight AdMob integration layer for Kivy4Admob on Android apps using Pyjnius. It supports banner ads, interstitial ads, and rewarded ads with full Java-to-Python callback support.

## Features

- ✅ Java event listener to receive ad status in Python
- ✅ Simple API with auto-threading for UI safety

---

## 🔧 Buildozer Setup
Make a local copy of admob4kivy.py , java_code folder in your project 

Make sure your Java code (e.g., `AdmobManager.java`, `AdmobListener.java`) is inside `./java_code/org/kivy/admob4kivy/`.

Then edit your `buildozer.spec` as follows:

```ini
# Java source directory
android.add_src = ./java_code

# Required permissions
android.permissions = INTERNET,ACCESS_NETWORK_STATE

# AdMob App ID (Test ID shown below; replace with your own production ID)
android.meta_data = com.google.android.gms.ads.APPLICATION_ID=ca-app-pub-3940256099942544~3347511713
android.enable_androidx = True

# Required AdMob + Firebase Ads SDK
android.gradle_dependencies = com.google.android.gms:play-services-ads:22.6.0,com.google.firebase:firebase-ads:21.4.0
```

You may also want to ensure:

```ini
requirements = python3,kivy,pyjnius,android
```

---

## Java Integration

- `AdmobManager.java`: Loads and shows ads using the Google Mobile Ads SDK.
- `AdmobListener.java`: Forwards Java AdMob events to Python using Pyjnius.

---





## Pay for Support

If you find this project helpful and want to support development, you can donate for support:

-  [![Support me on Ko-fi](https://img.shields.io/badge/Support%20me%20on-Ko--fi-%23FF5F5F.svg?style=flat&logo=ko-fi&logoColor=white)](https://ko-fi.com/sahilpixel)
  
- [![Donate with PayPal](https://img.shields.io/badge/Donate-PayPal-blue?style=flat&logo=paypal&logoColor=white)](https://paypal.me/SKSAHILIN?country.x=IN&locale.x=en_GB)


Thank you for your support!
---

## License

MIT License

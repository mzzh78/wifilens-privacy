# Privacy Policy for WiFiLens: Wi-Fi Cyber Defense

**Effective Date:** October 27, 2026  
**Last Updated:** October 27, 2026

AegisNet Technologies ("we", "our", or "us") is committed to protecting your privacy. This Privacy Policy outlines our data handling practices for the **WiFiLens: Wi-Fi Cyber Defense** mobile application.

---

### 1. 100% Zero-Cloud & Zero-Data Collection
WiFiLens is architected on a strict **Zero-Cloud, On-Device Local Processing** model:
- **No Personal Data Collected:** We do not collect, log, store, sell, or transmit any personally identifiable information (PII).
- **No Third-Party Analytics:** We do not integrate tracking, analytics, or behavioral telemetry SDKs (such as Google Firebase Analytics, Mixpanel, or Facebook SDK).
- **No Advertising:** WiFiLens contains zero advertising frameworks (such as Google AdMob, Unity, or AppLovin).
- **100% On-Device Execution:** All radio signal processing, optical viewfinder filters, and magnetic anomaly algorithms execute strictly in volatile memory on your local Android device.

---

### 2. Device Permissions Usage & Transparency
WiFiLens requires specific Android runtime permissions solely to interface with local hardware sensors. None of this data ever leaves your device:

- **Location (`ACCESS_FINE_LOCATION`, `ACCESS_COARSE_LOCATION`, `NEARBY_WIFI_DEVICES`):**  
  Required by Android OS architecture to perform 802.11 Wi-Fi radio scans (`WifiManager.getScanResults()`) and read SSID/BSSID metadata. **Your actual physical GPS location is never determined, stored, or transmitted.**
- **Camera & Flashlight (`CAMERA`, `FLASHLIGHT`):**  
  Utilized exclusively for the Optical Glint Lens Locator to pulse the hardware LED and detect retro-reflection glints from hidden pinhole camera lenses. **No video frames or photos are ever saved, recorded, or uploaded to any server.**
- **Audio (`RECORD_AUDIO`):**  
  Utilized exclusively by the Ultrasonic Acoustic Sentry to compute an in-memory Fast Fourier Transform (FFT) in the high-frequency 18 kHz to 22 kHz band. **No human voice or audible sound is ever recorded, stored, transcribed, or transmitted.**
- **Sensors (Magnetometer, Gyroscope):**  
  Utilized locally for 3D AHRS spatial positioning and magnetic anomaly bug detection (3D MAD).
- **Foreground Service (`FOREGROUND_SERVICE_LOCATION`, `FOREGROUND_SERVICE_CONNECTED_DEVICE`):**  
  Utilized only when the user explicitly starts the background Sentry mode to alert against rogue AP evil twin attacks. A persistent system notification is displayed at all times with a stop button.

---

### 3. Data Retention and Security
Because WiFiLens transmits zero data over the internet, your diagnostics and security audits are strictly confined to your local device. Any generated audit reports are saved exclusively in your device's local sandbox storage and can be deleted at any time by clearing the application storage (`Settings > Apps > WiFiLens > Clear Data`).

---

### 4. Children's Privacy
WiFiLens does not knowingly collect or solicit any information from anyone under the age of 13.

---

### 5. Contact & Inquiries
If you have any questions or concerns regarding this Privacy Policy, please contact our security team at:  
**Email:** `privacy@aegisnet-security.io`  
**GitHub:** [https://github.com/mzzh78/WifiLens](https://github.com/mzzh78/WifiLens)

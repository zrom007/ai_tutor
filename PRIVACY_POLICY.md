# Privacy Policy — Offline AI Language Tutor

**Last updated:** 2026-03-16  
**Version:** 1.0 (v0.1 release)  
**Contact:** [your-email@example.com] ← заменить перед публикацией

---

## TL;DR (plain language summary)

- We do **not** collect your name, email, or any account information.
- We do **not** run any servers that process your data.
- Your voice is processed **on your device** when possible. See STT section below.
- Your learning progress is stored **only on your device**.
- We use **crash reporting** (Firebase Crashlytics) — anonymous, no voice data.

---

## 1. What data we collect and why

### 1.1 Voice / Speech data (STT)

This app uses your device's **operating system speech recognition API** (Android SpeechRecognizer) to convert your spoken words into text.

**Important disclosure:**  
We use `preferOffline = true`, which instructs Android to use a locally installed speech model when available. However:

- If a local speech model is **not installed** on your device, Android may route the audio to **Google's cloud servers** for processing.
- We have **no control** over whether Android uses local or cloud processing in any given session.
- We do **not** receive, store, or have access to your voice recordings at any point.

**What this means for you:**
- Most modern Android devices (Android 10+) have a local speech model pre-installed.
- If you want to guarantee no audio leaves your device, you can verify your device has an offline speech model installed in: *Settings → General management → Language → Text-to-speech* (exact path varies by manufacturer).
- Audio processed by Google is subject to [Google's Privacy Policy](https://policies.google.com/privacy).

**We never store voice recordings.** The only output we use is the transcribed text string, processed entirely within the app.

### 1.2 Learning progress data

The following data is stored **locally on your device only**, in the app's private storage:

- Current learning level (A1–C2)
- Selected language pair (e.g., Russian → English)
- List of completed scenario IDs (to avoid repetition)
- Session history: date, fluency score per session (numeric, no text content)
- App preferences (TTS speed, etc.)

This data is **never transmitted** anywhere. It is deleted when you uninstall the app.

### 1.3 Crash reports (Firebase Crashlytics)

We use Firebase Crashlytics to receive anonymous crash reports when the app crashes unexpectedly. This helps us fix bugs.

**What Crashlytics collects:**
- Stack trace of the crash (code location, not user data)
- Device model and Android version
- App version
- A random installation ID (not linked to you personally)

**What Crashlytics does NOT collect:**
- Your voice or transcribed text
- Your learning history
- Any personally identifiable information

Crashlytics is a Google service. Data is processed according to [Google's Privacy Policy](https://policies.google.com/privacy) and [Firebase Data Processing Terms](https://firebase.google.com/terms/data-processing-terms).

### 1.4 Analytics (Firebase Analytics)

We collect anonymous usage events to understand how the app is used:

| Event | Data collected |
|---|---|
| `session_start` | Timestamp, language pair, level |
| `turn_completed` | Match/fallback result (boolean), turn index |
| `scenario_changed` | New scenario level — no scenario content |
| `fallback_triggered` | Count only |

**No voice data, no transcribed text, no personal identifiers** are included in any analytics event.

You can opt out of Analytics by enabling "Opt out of Ads Personalization" in your device's Google settings. This also disables Firebase Analytics collection.

### 1.5 Content updates (OTA)

When a new version of the scenario database is available, the app may download it in the background over Wi-Fi. The app will ask for your permission before downloading over mobile data.

**What is transmitted:** The scenario database file (`content_vX.db`). This is static content — it does not contain any of your personal data.

---

## 2. Data we do NOT collect

We explicitly do **not** collect:

- ❌ Name, email address, or any account information (no accounts exist)
- ❌ Voice recordings or audio files
- ❌ Transcribed text of your speech
- ❌ Location data
- ❌ Contacts, photos, or any other device data
- ❌ Advertising identifiers (we show no ads)

---

## 3. Data sharing

We do not sell, rent, or share your personal data with third parties, except:

- **Google** — via Android SpeechRecognizer (if cloud fallback occurs, outside our control) and Firebase services (Crashlytics, Analytics). See Google's Privacy Policy.
- **Legal requirements** — if required by law (we have no data to share beyond what's described above).

---

## 4. Data retention and deletion

| Data type | Location | Retention | How to delete |
|---|---|---|---|
| Learning progress | Your device | Until app uninstall | Uninstall app, or use in-app reset in Settings |
| Crash reports | Firebase servers | 90 days (Firebase default) | Not possible to delete individual reports — they contain no PII |
| Analytics events | Firebase servers | 14 months (Firebase default) | Opt out via device Google settings |

---

## 5. Children's privacy

This app is not directed at children under 13. We do not knowingly collect data from children. If you are a parent and believe your child has used this app, the only data that may exist is anonymous crash/analytics data, which cannot be linked to any individual.

---

## 6. GDPR (European Union users)

If you are located in the European Union:

- **Legal basis for processing:** Legitimate interest (crash reporting for app stability) and consent (analytics, which you can opt out of).
- **Your rights:** You have the right to access, correct, and delete data about you. Given we hold no personally identifiable data, the primary applicable right is to **opt out of analytics** (see Section 1.4).
- **Data transfers:** Firebase services transfer data to the United States. Google maintains Standard Contractual Clauses for GDPR compliance.
- **Contact for GDPR requests:** [your-email@example.com]

---

## 7. Changes to this policy

We will update this policy when the app's data practices change. The "Last updated" date at the top will reflect any changes. Continued use of the app after an update constitutes acceptance of the revised policy.

---

## 8. Contact

Questions about this Privacy Policy:  
📧 zrp1974@gmail.com 

---

*This Privacy Policy applies to the Android version of Offline AI Language Tutor (v0.1).*

# Qandeel Privacy Policy

**Effective date:** 26 November 2026
**App:** Qandeel – قنديل (iPhone, iPad and Apple Watch)
**Developer:** Adnan Altimeemy, independent developer, Manchester, United Kingdom

## The short version

- Qandeel has **no account, no ads, no analytics and no tracking**.
- **We do not collect, store, sell or share your personal data.** We have no server that receives it.
- Prayer times, the Qibla direction and the Hijri date are **calculated on your device**.
- Your records stay **on your devices**, and in **your own private iCloud account** if iCloud sync is on.
- Your **private journal never leaves the device it was written on**.
- Qandeel is free. There are no in-app purchases.

In App Store terms, Qandeel's privacy label is **Data Not Collected**.

---

## 1. Who we are

Qandeel is developed and published by Adnan Altimeemy, an independent developer based in Manchester, UK. For the purposes of UK GDPR and the EU GDPR, we would be the "controller" of any personal data we processed. Qandeel is designed so that we don't process any personal data at all.

## 2. Information that stays on your device

Qandeel stores the following **only on your device**, inside the app's private storage. We cannot see it.

| What | Why | Where it lives |
|---|---|---|
| Your first name, if you choose to enter one | A friendly greeting on Home | Your device only. It is not synced to iCloud |
| Your location (city name, latitude and longitude) | To calculate prayer times and the Qibla direction | Your device only. It is not synced to iCloud |
| Settings (calculation method, notifications, theme, language and similar) | To make the app work the way you set it up | Your device only |
| Prayer, fasting, Quran-reading, tasbih, good-deeds, taraweeh and Eid records; bookmarks and favourite duas | Your personal trackers | Your device, plus your private iCloud if sync is on (see section 4) |
| Private journal | Your personal reflections | **This device only**, protected by iOS Data Protection and optionally by Face ID or Touch ID. Never synced or backed up to us |
| Mosque timetables you import (CSV files) | To use your mosque's prayer, iqamah and Jumu'ah times | Your device only |
| Adhan recordings you import | To play your chosen adhan in notifications | Your device only |
| Downloaded Quran recitations and translations | To use them offline | Your device only |

You can delete this data at any time:
- **Prayer and fasting records:** *Settings ▸ Privacy ▸ Erase my prayer and fasting records*.
- **Downloaded recitations:** *Settings ▸ Quran ▸ Delete downloaded recitations*.
- **Imported adhan recordings:** *Settings ▸ Adhan sound ▸ Remove imported recordings*.
- **Imported timetable:** *Match my mosque ▸ Remove timetable*.
- **Everything:** delete the app.

### Location

Qandeel asks for **"While Using the App"** location access, and only if you choose **Use my current location**. You can instead search for your town by name, or decline location access completely.

- Your coordinates are used **on the device** to calculate prayer times and the Qibla direction.
- To show the name of your town, Qandeel uses Apple's geocoding service (`CLGeocoder`). Apple receives the coordinates or the place name you searched for and returns a place name. This is governed by [Apple's Privacy Policy](https://www.apple.com/legal/privacy/). We do not receive it.
- Qandeel does **not** track your location in the background and never sends your location to us or to any other service.

### Face ID / Touch ID

If you lock your journal, iOS checks your face or fingerprint. Qandeel only receives a yes or no answer. Biometric data never leaves Apple's Secure Enclave and is never available to Qandeel.

## 3. Online services Qandeel connects to

Some optional features download content from public services. These requests contain **no personal information from Qandeel**: no name, no location, no identifiers and no records. As with any internet request, the service can see your device's **IP address** and **what was requested**, for example "Surah 18, Pickthall translation".

| Service | When it's used | What's requested | Their privacy information |
|---|---|---|---|
| **Al Quran Cloud** (`api.alquran.cloud`), with audio served from the Islamic Network CDN (`cdn.islamic.network`) | When you choose a translation that isn't built in, or play or download a recitation | The surah number, translation or reciter | [alquran.cloud](https://alquran.cloud) / [islamic.network](https://islamic.network) |
| **Quran.com API** (`api.quran.com`) | When you turn on word-by-word meanings | The surah number and language | [quran.com/privacy](https://quran.com/privacy) |
| **Apple** (geocoding, iCloud, notifications, Siri, Apple Watch) | As described in sections 2 and 4 | As described | [apple.com/legal/privacy](https://www.apple.com/legal/privacy/) |

The Arabic Quran text, the Saheeh International and Maududi translations, the duas, the hadith, the guides and Ask Qandeel are **built into the app** and work without an internet connection.

**Ask Qandeel** searches only the content built into the app, **on your device**. Your questions are not sent anywhere and are not saved.

## 4. iCloud sync

If **Sync with iCloud** is on (*Settings ▸ iPhone & iPad sync*), Qandeel keeps your trackers, bookmarks and favourites in step between your devices. It uses Apple's iCloud key-value storage in **your own iCloud account**.

- We cannot access your iCloud data.
- **Not synced:** your location, your settings, imported files and your **private journal**.
- To stop syncing, turn the toggle off. To remove synced data from iCloud, go to *iOS Settings ▸ [your name] ▸ iCloud ▸ Manage Account Storage*.

## 5. Apple Watch, widgets, Live Activities and Siri

- **Apple Watch:** your iPhone sends today's prayer times and your prayer ticks to your Watch directly, using Apple's WatchConnectivity. Nothing passes through us.
- **Widgets and Live Activities:** these read data that Qandeel shares with its own widgets on your device, through an App Group. They may show prayer times on your Lock Screen; you can turn this off at any time.
- **Siri and Shortcuts:** when you ask Siri about Qandeel, Apple processes the request under its own privacy policy. Qandeel answers on your device.

## 6. Notifications

Prayer reminders are **scheduled on your device** using iOS local notifications. Qandeel does not use push notifications, so no device token is ever sent to a server.

## 7. Sharing

Qandeel shares something only when **you** tap a Share button, for example a dua, a verse, your monthly timetable or your Ramadan summary card. You choose where it goes, using the standard iOS share sheet.

## 8. What Qandeel does not do

- No advertising, and no advertising identifier (IDFA).
- No analytics, crash-reporting or tracking SDKs.
- No account or sign-in.
- No selling, renting or sharing of data with anyone.
- No in-app purchases or payment information.

Qandeel's privacy manifest (`PrivacyInfo.xcprivacy`) is included in this repository. It declares no tracking and no collected data types.

## 9. Children

Qandeel is suitable for all ages and collects no personal information from anyone, including children.

## 10. Your rights

Under UK GDPR and the EU GDPR you have rights to access, correct, delete and port your personal data. Because Qandeel doesn't send your data to us, **we hold no personal data about you**. All your data is under your control, on your devices and in your iCloud account, and you can view, change or delete it as described above. If you contact us by email, we use your message only to reply, and delete it once the matter is resolved.

If you have a concern, you can also contact the UK Information Commissioner's Office at [ico.org.uk](https://ico.org.uk).

## 11. Changes to this policy

If Qandeel's handling of data changes, this policy will be updated and the effective date above will change. The full history is available in this repository's commit history. Material changes will also be mentioned in the app's release notes.

## 12. Contact

- **GitHub:** open an issue in this repository. Please don't post personal information in a public issue.
- **Email:** `[your contact email]`

<div align="center">

# Qandeel – قنديل

**Your Faith. Your Life. Your Light.**

An all-in-one Muslim lifestyle app for **iPhone, iPad and Apple Watch**: prayer times, Qibla, the Quran, duas, the Islamic calendar and personal trackers, in one calm and private place.

English · العربية · اردو  |  iOS 17+ · watchOS 10+  |  **Free: no ads, no account, no tracking**

[User Guide](USER_GUIDE.md) · [Privacy Policy](PRIVACY.md) · Report an issue to adnanaltimeemy@outlook.com 

</div>

---

## Features

**Prayer**
- Accurate prayer times calculated on the device, with 10 calculation methods, Standard or Hanafi Asr, high-latitude rules for the UK and other northern countries, and per-prayer adjustments.
- **Match my mosque:** import your mosque's CSV timetable, including **iqamah** and **Jumu'ah** times.
- Reliable reminders: an optional alert 5–30 minutes before each prayer, a suhoor alarm, and Jumu'ah and iqamah reminders. You can import your own licensed adhan recording.
- A **Qibla compass**, a **prayer tracker** with make-up (qada) prayers, and a monthly timetable you can export.

**Quran**
- The full Uthmani text, with **Saheeh International** (English) and **Maududi** (Urdu) translations, built in and **working offline**.
- Recitations from seven reciters with verse highlighting and offline downloads, **word-by-word** meanings, **memorisation mode**, bookmarks and a **khatm planner**.

**Daily life**
- **Duas** by occasion, with Arabic, transliteration, translation and source. **Tasbih** counter.
- **Islamic calendar** with events, fasting tracker, fasting guide, Eid guide and checklist, and a reading tracker.
- **Ramadan:** suhoor and iftar times, a taraweeh tracker and a shareable summary card.
- **Wudu and prayer guides**, a **good deeds** tracker and a **private journal** with a Face ID lock.
- **Ask Qandeel:** searches the built-in Quran, hadith, duas and guides on your device, and shows passages exactly as they appear in their source, with references. It never generates religious text or issues rulings.

**Apple features**
- Home Screen and Lock Screen **widgets** with tick-off buttons.
- **Live Activity** and **Dynamic Island** countdown to the next prayer, or to iftar.
- An **Apple Watch** app with complications.
- **Siri** and **Shortcuts**: "When is Asr in Qandeel?"
- **iCloud sync** between iPhone and iPad. The journal is never synced.
- **Dynamic Type**, VoiceOver (with Arabic read by an Arabic voice) and full **right-to-left** layout for Arabic and Urdu.

See the **[User Guide](USER_GUIDE.md)** for how to use everything.

## Privacy

Qandeel has no account, no ads, no analytics and no tracking SDKs, and **collects no personal data**. Prayer times and the Qibla are calculated on your device. Your records stay on your devices and, if you turn on sync, in your own private iCloud. App Store privacy label: **Data Not Collected**.

Read the full **[Privacy Policy](PRIVACY.md)**.

## Our principles

- **Sources, not opinions.** Every verse, hadith, dua and guide point shows its reference. We never write or paraphrase religious text as if it were a quotation.
- **No fatwas.** Where scholars differ, Qandeel says so. For personal rulings, please ask a qualified scholar.
- **Faith is not a score.** Trackers are private tools for consistency, not leaderboards. Qandeel is free, with no features locked behind payment.
- **Reviewed before release.** Religious content and translations are checked by qualified reviewers.

## Building from source

**Requirements:** Xcode 15 or later (Xcode 16 recommended), iOS 17 and watchOS 10 SDKs.

1. Clone the repository and open **`NOOR.xcodeproj`**. (NOOR was the app's working title, so the project, targets and folders keep that name; users only ever see **Qandeel**.)
2. Select the **NOOR** project, then go to **Build Settings ▸ User-Defined** and set **`APP_BUNDLE_ID`** to an identifier you own (default `com.adnanaltimeemy.noor`). Every target's bundle ID and the App Group (`group.$(APP_BUNDLE_ID)`) are derived from it.
3. Set your **Team** on the **NOOR**, **NOORWidget**, **NOORWatch** and **NOORWatchWidget** targets. Automatic signing adds the capabilities: App Groups, iCloud key-value storage, Time Sensitive Notifications and Background Modes.
4. Run the **NOOR** scheme on an iPhone, iPad or Simulator. Use **NOORWatch** to run on Apple Watch.
5. Press **⌘U** to run the unit and UI tests.

**Tips**
- **Simulator location:** use *Features ▸ Location*. On a device run from Xcode, make sure *Debug ▸ Simulate Location* is off.
- **App language:** test Arabic and Urdu with *Scheme ▸ Run ▸ Options ▸ App Language*.

### Project layout

```
NOOR.xcodeproj        Targets: NOOR, NOORWidget, NOORWatch, NOORWatchWidget, NOORTests, NOORUITests
Shared/               Prayer engine, Qibla, Hijri, mosque timetables, storage + iCloud sync,
                      themes, widget intent, Live Activity attributes, Watch payload, strings
NOOR/                 iPhone & iPad app (App, Models, Services, Content, Intents, Views, Resources)
NOORWidget/           Home & Lock Screen widgets, Live Activity / Dynamic Island
NOORWatch/            Apple Watch app
NOORWatchWidget/      Watch-face complications
NOORTests/            Unit tests (prayer times, Qibla, notifications, CSV import, Ask Qandeel, sync)
NOORUITests/          UI and App Store screenshot tests
fastlane/metadata/    App Store listing (en-GB, ar-SA, ur)
docs/                 Launch checklist and content review packs
.github/workflows/    CI (GitHub Actions); ci_scripts/ for Xcode Cloud
```

**Tech:** SwiftUI with Observation, WidgetKit, ActivityKit, App Intents, WatchConnectivity, CoreLocation, AVFoundation, LocalAuthentication, NSUbiquitousKeyValueStore and String Catalogs. Qandeel has **no third-party dependencies**.

## Content sources and credits

| Content | Source | Licence / terms |
|---|---|---|
| Quran Arabic text | [Tanzil Project](https://tanzil.net), Uthmani text, unmodified | CC BY 3.0 |
| English translation | Saheeh International, via [QuranEnc](https://quranenc.com) | Per QuranEnc / rights holder terms |
| Urdu translation | Abul A'la Maududi, via [QuranEnc](https://quranenc.com) | Per QuranEnc / rights holder terms |
| Other translations and recitations | [Al Quran Cloud API](https://alquran.cloud) | Per provider terms |
| Word-by-word meanings | [Quran.com API](https://quran.com) | Per provider terms |
| Hadith Arabic text | Open hadith-json dataset (text from [Sunnah.com](https://sunnah.com)) | Per dataset / source terms |
| Quran fonts | KFGQPC Uthmanic Script HAFS ([King Fahd Complex](https://fonts.qurancomplex.gov.sa)); [Amiri Quran](https://github.com/aliftype/amiri) | KFGQPC terms; SIL Open Font License 1.1 |
| Prayer-time algorithm | Based on [PrayTimes.org](http://praytimes.org) | Re-implemented in Swift |
| Hijri calendar | Umm al-Qura (Apple Foundation) | — |

Third-party content remains under its original licence and terms. Please keep these attributions if you reuse it.

## Contributing

Issues and suggestions are welcome.

- **Bugs:** please include your device, iOS version, Qandeel version and the steps to reproduce.
- **Content corrections:** if you find an error in a verse, translation, hadith, dua or reference, open an issue and include the reference. Religious content changes are checked by qualified reviewers before they are merged.
- **Translations:** native Arabic and Urdu speakers are especially welcome to review the strings in `Shared/Localizable.xcstrings`.

## Licence

The source code is © 2026 Adnan Altimeemy. No open-source licence is granted unless a `LICENSE` file is added to this repository. The third-party content listed above is covered by its own licences.

---

<div align="center">
Made in Manchester, UK · Jazakallah khairan (جَزَاكَ اللَّهُ خَيْرًا) for using Qandeel
</div>
# Qandeel

# Debloat-OneUi-Lite
## What is Debloat?

**Debloating** is the process of removing or disabling pre-installed applications and system components that are not needed by the user. These packages may be installed by the device manufacturer, mobile carrier, Google, or third-party partners.

The purpose of debloating is usually to reduce unwanted applications, limit unnecessary background activity, simplify the app drawer, and give the user more control over the device.

The accompanying script uses:

```sh
pm uninstall -k --user 0 <package.name>
```

This command removes the selected package for Android user `0`, which is normally the primary device user. The `-k` option keeps the package data and cache. This is a user-level removal, not a complete deletion of the package from the system partition. A system package may be restored with:

```sh
cmd package install-existing --user 0 <package.name>
```

The package list below contains **93 unique packages** included in `lite.sh`. Application names are common names or functional descriptions. The exact display name may vary by device model, Android version, Samsung One UI version, carrier, and region. Some entries are system services and do not have a separate app icon.

## Removed Package Summary

| # | Package name | Common application or function |
|---:|---|---|
| 1 | `com.netflix.mediaclient` | Netflix |
| 2 | `com.samsung.android.mobileservice` | Samsung Mobile Service |
| 3 | `com.osp.app.signin` | Samsung Account / Samsung Login |
| 4 | `com.samsung.android.scloud` | Samsung Cloud |
| 5 | `com.google.android.projection.gearhead` | Android Auto |
| 6 | `com.samsung.android.bixby.agent` | Bixby |
| 7 | `com.samsung.android.app.settings.bixby` | Bixby Settings Integration |
| 8 | `com.microsoft.appmanager` | Link to Windows / Microsoft Phone Link Service |
| 9 | `com.samsung.android.app.tips` | Samsung Tips |
| 10 | `com.sec.android.daemonapp` | Samsung Weather Service |
| 11 | `com.samsung.android.themestore` | Galaxy Themes / Theme Store |
| 12 | `com.android.printspooler` | Android Print Spooler |
| 13 | `com.android.bprint` | Built-in Print Service |
| 14 | `com.facebook.services` | Facebook Services |
| 15 | `com.facebook.system` | Facebook System Service |
| 16 | `com.samsung.android.bixbyvision.framework` | Bixby Vision Framework |
| 17 | `com.samsung.android.smartmirroring` | Smart View / Smart Mirroring |
| 18 | `com.sec.android.app.magnifier` | Magnifier |
| 19 | `com.google.android.apps.restore` | Android Restore Service |
| 20 | `com.samsung.android.aware.service` | Samsung Awareness Service |
| 21 | `com.samsung.android.app.omcagent` | Samsung OMC Agent / Carrier Configuration |
| 22 | `com.samsung.android.mapsagent` | Samsung Maps Agent |
| 23 | `com.sec.android.app.quicktool` | Samsung Quick Tools |
| 24 | `com.sec.android.app.billing` | Samsung Billing |
| 25 | `com.samsung.android.stickercenter` | Samsung Sticker Center |
| 26 | `com.samsung.app.newtrim` | Samsung Video Trimmer |
| 27 | `com.samsung.android.visualars` | Samsung Visual AR |
| 28 | `com.google.android.apps.docs.editors.sheets` | Google Sheets |
| 29 | `com.google.mainline.adservices` | Google Ad Services |
| 30 | `com.google.android.adservices.api` | Android/Google AdServices API |
| 31 | `com.android.bookmarkprovider` | Android Bookmark Provider |
| 32 | `com.android.dreams.basic` | Basic Daydream / Basic Screen Saver |
| 33 | `com.android.dreams.phototable` | Photo Table Screen Saver |
| 34 | `com.android.egg` | Android Easter Egg |
| 35 | `com.android.hotwordenrollment.okgoogle` | Voice Match: “OK Google” |
| 36 | `com.android.hotwordenrollment.xgoogle` | Google Hotword Enrollment |
| 37 | `com.google.android.providers.partnerbookmarks` | Google Partner Bookmarks |
| 38 | `com.sec.android.app.samsungapps` | Galaxy Store |
| 39 | `com.samsung.android.dynamiclock` | Dynamic Lock Screen |
| 40 | `com.samsung.android.tvplus` | Samsung TV Plus |
| 41 | `com.samsung.android.app.watchmanagerstub` | Galaxy Watch Plugin Stub |
| 42 | `com.samsung.android.app.watchmanager` | Galaxy Wearable / Galaxy Watch Manager |
| 43 | `com.samsung.android.waterplugin` | Samsung Water Plugin |
| 44 | `com.samsung.android.accessibility.talkback` | Samsung TalkBack / Screen Reader |
| 45 | `com.samsung.android.bixby.wakeup` | Bixby Voice Wake-up |
| 46 | `com.sec.android.app.shealth` | Samsung Health |
| 47 | `com.samsung.android.arzone` | AR Zone |
| 48 | `com.google.android.apps.docs` | Google Drive |
| 49 | `com.google.android.apps.tachyon` | Google Duo / Legacy Google Meet |
| 50 | `com.google.android.feedback` | Google Feedback |
| 51 | `com.google.android.googlequicksearchbox` | Google App / Google Search |
| 52 | `com.google.android.marvin.talkback` | Android Accessibility Suite / Google TalkBack |
| 53 | `com.google.android.printservice.recommendation` | Print Service Recommendations |
| 54 | `com.google.android.syncadapters.calendar` | Google Calendar Sync |
| 55 | `com.google.android.tts` | Speech Services by Google / Text-to-Speech |
| 56 | `com.google.android.apps.youtube.music` | YouTube Music |
| 57 | `com.google.ar.core` | Google Play Services for AR / ARCore |
| 58 | `com.sec.android.mimage.avatarstickers` | AR Emoji Stickers |
| 59 | `com.samsung.android.aremojieditor` | AR Emoji Editor |
| 60 | `com.android.bips` | Built-in Print Service |
| 61 | `com.samsung.android.game.gametools` | Game Booster / Game Tools |
| 62 | `com.samsung.android.game.gos` | Game Optimizing Service (GOS) |
| 63 | `com.samsung.android.kidsinstaller` | Samsung Kids Installer |
| 64 | `com.samsung.android.app.camera.sticker.facearavatar.preload` | Camera AR Avatar and Face Sticker Preload |
| 65 | `com.sec.android.app.sbrowser` | Samsung Internet |
| 66 | `com.sec.android.easyMover.Agent` | Smart Switch / Easy Mover |
| 67 | `com.samsung.android.calendar` | Samsung Calendar |
| 68 | `com.sec.android.dexsystemui` | Samsung DeX System UI |
| 69 | `com.sec.android.app.desktoplauncher` | Samsung DeX Home / Desktop Launcher |
| 70 | `com.synchronoss.dcs.att.r2g` | AT&T Ready2Go / Carrier Setup Service |
| 71 | `com.wavemarket.waplauncher` | Carrier WAP Launcher |
| 72 | `com.pandora.android` | Pandora |
| 73 | `com.sec.penup` | PENUP |
| 74 | `com.wb.goog.got.conquest` | Game of Thrones: Conquest |
| 75 | `com.foxnextgames.m3` | Marvel Strike Force |
| 76 | `com.microsoft.skydrive` | Microsoft OneDrive |
| 77 | `com.claromusica` | Claro Música |
| 78 | `com.clarovideo` | Claro video |
| 79 | `com.clarocloud` | Claro cloud |
| 80 | `com.claroshop` | Claro shop |
| 81 | `com.claropay` | Claro Pay |
| 82 | `com.claro.tv` | Claro TV |
| 83 | `com.claro.empresas` | Claro Empresas |
| 84 | `com.claro.assistant` | Claro Assistant |
| 85 | `com.claro.photoeditor` | Claro Photo Editor |
| 86 | `com.samsung.android.fmm` | Samsung Find My Mobile |
| 87 | `com.sec.android.app.ve.vebgm` | Samsung Video Editor Background Music |
| 88 | `com.claro.store` | Claro Store |
| 89 | `com.samsung.android.bixby.esdk.globalconstant` | Bixby ESDK Global Constants |
| 90 | `com.samsung.android.bluelightfilter` | Blue Light Filter |
| 91 | `com.samsung.android.app.sharelive` | Samsung ShareLive / Sharing Service |
| 92 | `com.sec.android.app.fm` | Samsung FM Radio |
| 93 | `com.samsung.android.themecenter` | Samsung Theme Center |

## Important Note

Removing a package can disable related features. Packages related to printing, accessibility, text-to-speech, Google Search, Samsung Account, Smart View, Samsung DeX, Galaxy Watch, Samsung Health, Samsung Internet, Calendar, and Game Booster should only be removed if those features are not needed.
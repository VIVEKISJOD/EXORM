<h1 align="center">EXORM</h1>

<p align="center">
Customers, follow-ups, quotations, events and payments for decoration and event businesses.<br>
Works fully offline on your Android phone. Free. No account. No ads.
</p>

<p align="center">
<a href="https://github.com/VIVEKISJOD/EXORM/releases/latest"><b>⬇ Download the latest EXORM.apk</b></a>
</p>

---

## What EXORM does

- **Customers**: save name, phone, requirement and budget. Warns you if a phone number is already saved.
- **Follow-ups**: Today, Overdue, Upcoming, Completed and Not interested lists. Tap the call button to open the phone dialer. Delete any follow-up you don't need.
- **Messages**: ready WhatsApp message templates you can edit. Nothing is ever sent automatically.
- **Quotations**: build a quote with items, discount and tax, keep every revision, and share it as a PDF or text.
- **Events and calendar**: month calendar, event type, venue, status, more than one event date, and an event follow-up date.
- **Payments**: agreed amount, advance taken, more payments, and the balance left to receive.
- **Equipment collection**: after an event, schedule and tick off the equipment you must collect back, with missing and damaged counts.
- **Add-ons**: turn features on or off for your type of business (Settings → Add-ons).
- **Reminders**: phone notifications for follow-ups, events and collections.
- **Backup**: save all your data to a file and restore it later. Export customers as CSV.
- **Look**: pure black screen with glass cards, easy on the eyes and the battery.

## Install

1. On your Android phone, open the **[latest release](https://github.com/VIVEKISJOD/EXORM/releases/latest)**.
2. Under **Assets**, tap **EXORM.apk** to download it.
3. Open the downloaded file and tap **Install**.
4. If Android says installs are blocked, tap **Settings** and allow installs from your browser or file manager, then go back and tap **Install** again.

Needs Android 8.0 or newer.

## Updates

When a new version is released, EXORM shows **Update available** when you open it.

1. Tap **Download & install**. The update downloads inside the app.
2. The first time, Android asks you to allow installs from EXORM. Turn it on once.
3. Tap **Install** on the Android screen.

Your data is kept when you update. You can also check by hand in **Settings**.

## Your data

- Everything is saved only on your phone. Nothing is uploaded anywhere.
- The only internet use is checking for and downloading updates from this page.
- Make a backup now and then (Settings → Backup). **Backups are not encrypted**, so keep the file somewhere safe.
- Uninstalling the app deletes its data. Restore from your backup if you reinstall.

## Permissions

| Permission | Why |
|---|---|
| Notifications | Follow-up, event and collection reminders |
| Internet | Check for and download updates |
| Install apps | Install the update you downloaded |
| Run at start-up | Bring your reminders back after the phone restarts |

## Coming later

Inventory, reports, global search, equipment photos.

## Problems or ideas

Open an **[Issue](https://github.com/VIVEKISJOD/EXORM/issues)** on this page and say what happened.

---

## For the owner: how this repo builds the app

You never need a computer.

1. Upload the new `EXORM.zip` to the repo root (**Add file → Upload files → Commit changes**).
2. **GitHub Actions** builds the app by itself (Actions tab, about 5 minutes).
3. When the run shows a green tick, a new **Release** appears with `EXORM.apk`.
4. People who already have the app see the update the next time they open it.

Notes:
- Keep this repo **public**. The in-app updater reads the releases without a login.
- The build file is `.github/workflows/build.yml`. Each build gets the next version number automatically (1.0.1, 1.0.2, ...).
- The app is signed with `exorm-release.jks` in the repo, so every update installs over the old one. Do not delete it.
- For people who want the code: Kotlin + Jetpack Compose, package `com.exorm.app`, Android 8.0+. `EXORM_HANDOFF.md` explains how the code is organised.
- This is made for direct install from GitHub, not for the Play Store.

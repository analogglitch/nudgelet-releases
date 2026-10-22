# Nudgelet privacy policy

Applies to the Nudgelet public beta for Mac and Android. Last updated 2026-10-22.

**Short version:** everything you put into Nudgelet stays on your own devices. There are no accounts, no analytics, no ads and no AI services. Nudgelet only uses the network if you pair your phone with your Mac, or if you tap "Check product" on a wishlist item.

## What Nudgelet stores, and where

Nudgelet saves the following **only on your device**:

- tasks, notes, tags, checklists and due times;
- photos, drawings and audio notes you attach;
- wishlist items, with any link, price and reason you add;
- focus sessions, points, your companion choices and your settings.

| Where | Location |
|---|---|
| Mac | `~/Library/Application Support/Nudgelet` |
| Android | the app's private storage |

Nudgelet does not encrypt this data separately. It is protected by your device's own lock and disk encryption. Android's automatic cloud backup is turned off for Nudgelet, so your data is not copied to Google.

## What leaves your device

Nothing leaves your device unless you use one of these two features.

1. **Syncing your phone with your Mac (off by default).**
   - What happens: when you pair a phone under Settings → Advanced, the phone and the Mac send your Nudgelet data directly to each other over your own Wi-Fi. No cloud server or third party is involved.
   - What to know: **this connection is not encrypted.** Anyone on the same network who is technically able to watch the traffic could read it. Only use it on your own home Wi-Fi, never on public, work or guest networks.
   - How to turn it off: "Forget paired devices" on the Mac disconnects every phone.
2. **"Check product" on a wishlist item.**
   - What happens: your Mac downloads the public product catalog from michifinds.com and looks for your item on the Mac.
   - What to know: your link, your list and your personal data are not sent. MichiFinds receives a normal web request, which includes your internet (IP) address.
   - On a phone: the check only works while the phone is paired with your Mac, and the Mac makes the request.

Opening a saved product link opens it in your browser, which then talks to that website directly.

## Device permissions

| Permission | Why | If you say no |
|---|---|---|
| Notifications (Android) | To show reminders for tasks with a due time. Reminders are silent. | No reminders on the phone. Everything else works. |
| Alarms & reminders (Android) | To deliver reminders at their exact time. | Reminders may arrive a few minutes late. |
| Microphone (Mac and Android) | Only when you tap Record audio for a task. Audio stays on your device; nothing is transcribed or uploaded. | Recording is unavailable. You can still attach an audio file. |

Two features use your phone's own apps instead of a Nudgelet permission:
- **Camera:** taking a photo opens the phone's camera app.
- **Voice input:** typing by voice uses your phone's speech service, under that service's own privacy terms.

## Backups

**Export a backup** (Settings → Your data) saves a JSON file that holds all your Nudgelet data in readable form. Keep it somewhere private.

## Deleting your data

- **Removing a single item:** deleting a task or attachment hides it. In this beta a record of it stays in the app's internal history and in exported backups, so your devices can stay in sync.
- **Removing everything on Mac:** quit Nudgelet from the menu bar, then delete `~/Library/Application Support/Nudgelet`.
- **Removing everything on Android:** uninstall Nudgelet, or go to Settings → Apps → Nudgelet → Storage → Clear storage.
- **Paired devices:** each device keeps its own copy until you remove it there too.

## Children

Nudgelet is not directed at children under 13.

## Changes and contact

Any change to this policy will appear in the release notes, with a new "last updated" date. Questions: open an issue at [github.com/analogglitch/nudgelet-releases/issues](https://github.com/analogglitch/nudgelet-releases/issues). Please never attach a backup file, because it contains your personal data.

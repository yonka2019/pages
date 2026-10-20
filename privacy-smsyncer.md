Privacy Policy — SMSyncer

Effective 21 October 2026

SMSyncer (com.yapps.smsyncer) is an Android app by y-apps. It turns incoming SMS that contain text you choose into tasks in your own Todoist project.

We collect nothing. There is no account with us and we run no server. The app has no analytics, no ads and no crash reporting.

What the app reads

┌──────────────────────────┬───────────────────────────────────┬───────────────────────────────────────────────────────────────────────┐
│           Data           │                Why                │                             Where it goes                             │
├──────────────────────────┼───────────────────────────────────┼───────────────────────────────────────────────────────────────────────┤
│ Incoming SMS (text)      │ To check it against your keywords │ Checked on your device. A non-matching SMS is ignored and not stored. │
├──────────────────────────┼───────────────────────────────────┼───────────────────────────────────────────────────────────────────────┤
│ Matching SMS (text only) │ To create your task               │ Sent to Todoist (see below)                                           │
└──────────────────────────┴───────────────────────────────────┴───────────────────────────────────────────────────────────────────────┘

The sender's number and the time are not sent anywhere.

Data sent off your device

Only to Todoist (api.todoist.com, run by Doist), and only after you enter your own Todoist API token:

- The full text of each matching SMS, which becomes a task in the project you picked.
- A request for your Todoist project list, so you can pick a project.

Everything goes over HTTPS. Once a task is in Todoist, Todoist's privacy policy applies to it: https://doist.com/privacy

The data goes to no other party. We do not sell or share data.

Data stored on your device

Kept in the app's private storage. Only SMSyncer can read it:

- Your Todoist API token, encrypted with a key held in the Android Keystore.
- The selected project (ID and name), your keywords and the on/off setting.
- The last 20 matching SMS texts, with their send status and time.

Android backup and device transfer are turned off for this app. To delete all of it, clear the app's data or uninstall the app. Tasks already created stay in Todoist until you delete them there.

Permissions

┌─────────────────────────────────────────────────────────────────────────────┬────────────────────────────────────────────────────────────────────────────────────────────────────────────┐
│                                 Permission                                  │                                                  Purpose                                                   │
├─────────────────────────────────────────────────────────────────────────────┼────────────────────────────────────────────────────────────────────────────────────────────────────────────┤
│ RECEIVE_SMS                                                                 │ Notice new SMS so they can be checked against your keywords.                                               │
├─────────────────────────────────────────────────────────────────────────────┼────────────────────────────────────────────────────────────────────────────────────────────────────────────┤
│ INTERNET                                                                    │ Talk to Todoist.                                                                                           │
├─────────────────────────────────────────────────────────────────────────────┼────────────────────────────────────────────────────────────────────────────────────────────────────────────┤
│ ACCESS_NETWORK_STATE, WAKE_LOCK, RECEIVE_BOOT_COMPLETED, FOREGROUND_SERVICE │ Added by Android's WorkManager so a queued SMS is sent once the network is back, including after a reboot. │
└─────────────────────────────────────────────────────────────────────────────┴────────────────────────────────────────────────────────────────────────────────────────────────────────────┘

Children

The app is not directed at children under 13 and does not knowingly process their data.

Changes

Any change is published on this page and the date above is updated.

Contact

yonka2003@gmail.com

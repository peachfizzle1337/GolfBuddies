# Golf Buddies iOS app (Capacitor)

Wraps the web app (`../index.html`) as an iOS app. It uses the same Supabase backend over the network, so all functionality is identical to the website.

## Update the app after editing `../index.html`

```sh
npm install      # first time / after a fresh clone
npm run sync     # copies ../index.html into the app
```

Then press Run in Xcode again.

## Open in Xcode

```sh
npm run open
```

## Install on the iPhone

1. Connect the iPhone by cable, unlock it, and tap "Trust this computer".
2. In Xcode, pick the iPhone in the device menu at the top, then press Run (▶).
3. First install only:
   - iPhone: Settings → Privacy & Security → Developer Mode → On (restarts the phone).
   - After installing: Settings → General → VPN & Device Management → trust "Apple Development: marcel_loegl@web.de".

## Notes

- Signing uses the free Personal Team (CKZRD6RC87). The app stops opening after 7 days; reconnect and press Run again to renew it.
- A free team can have at most 3 of your own apps on a device at once (FRIST counts as one).
- The app needs internet (Supabase, supabase-js, Chart.js and fonts load online).

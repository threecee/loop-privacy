# MyLoop With Watch — Privacy Policy

_Last updated: 2026-05-01_

MyLoop With Watch is a personal fork of the open-source Loop closed-loop
insulin delivery app, with an Apple Watch companion app for use during
overnight separation from the iPhone. Distributed via Apple TestFlight
Internal Testing for personal use only.

## What data we collect (locally on your devices)

- **Apple HealthKit data**: blood glucose readings (from your CGM),
  insulin delivery records (from your pump), carbohydrate entries, and
  related health-and-fitness samples. Loop reads these to compute closed-loop
  decisions and writes back the resulting insulin doses.
- **Bluetooth pump telemetry**: pod state, insulin reservoir level,
  pump alerts, sensor calibration values. Stored on-device only; required
  for pump operation.
- **Device identifiers**: CGM transmitter serial number, insulin pump
  pod serial number — required for Bluetooth pairing.

## What data we may send off-device (only with your explicit configuration)

- **Nightscout** (optional): if you've configured a Nightscout endpoint
  in app settings, MyLoop With Watch sends glucose, insulin, and pump
  telemetry to your own self-hosted Nightscout instance for review and
  remote monitoring. We do not provide a Nightscout server; this is your
  infrastructure.

## What we do NOT collect

- We do not use third-party analytics, ad SDKs, or telemetry services
  (no Crashlytics, Firebase, Sentry, etc.).
- We do not send any data to a server we operate. There is no MyLoop
  backend; the app is fully offline-capable.
- We do not sell, rent, or share your data with anyone.
- We do not collect data via the watch app independently — the watch
  syncs with the iPhone via WatchConnectivity (Apple's encrypted
  on-device peer-to-peer transport).

## Where data lives

- **Your iPhone**: HealthKit (encrypted at rest by iOS), Loop's local
  Core Data store, and shared App Group container.
- **Your Apple Watch**: a mirrored subset of Loop state (active basal,
  pod status, recent glucose readings) for offline operation when
  separated from the iPhone.
- **Your CGM transmitter and insulin pump**: the device firmware
  retains its own state (glucose readings, dose history) per
  manufacturer specifications.
- **Your Nightscout server** (if configured): per your Nightscout
  privacy policy.

## Your rights

- You can disable Nightscout sync at any time in app settings.
- You can revoke HealthKit permissions at any time in iOS Settings →
  Privacy & Security → Health → MyLoop With Watch.
- You can uninstall the app at any time, which removes all local
  Loop data (HealthKit data persists per Apple's policy).
- You can request deletion of your Nightscout server data per your
  Nightscout server's policy.

## Children

MyLoop With Watch is intended for adult users managing their own
closed-loop insulin delivery, OR for adult parents/guardians configuring
the app on a minor child's iPhone with HealthKit linked to the child's
Apple ID. The app does not have separate child-account flows.

## Liability

This is a personal fork of an open-source community-maintained app and
is **not a regulated medical device**. The Loop algorithm has not
been reviewed or approved by the FDA, EMA, or any other regulatory
body. This app is for personal use by individuals who understand the
risks of using non-regulated closed-loop insulin delivery software.
**Do not use this app without consulting your endocrinologist and your
care team.**

## Contact

Carl Christian Christensen — carl.christian.christensen@gmail.com

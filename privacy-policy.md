# Swoop Privacy Policy

_Last updated: 14 May 2026_

Swoop is built around a simple promise: your photos never leave your device. This page describes exactly what data Swoop touches, what stays on-device, and the few cases where third parties may be involved.

## What Swoop accesses on your device

- **Photo library.** Swoop requests access to your iPhone's photo library so it can show you photos and videos for triage. You can grant either full access or limited (selected photos) access. With limited access, Swoop only sees the photos you pick.
- **Photo metadata.** Swoop reads each photo's creation date, location (if you've allowed Photos to embed it), burst identifier, and similar attributes provided by Apple's PhotoKit framework. This is used to group similar photos and order them chronologically.

## What Swoop does with your photos

All processing happens **locally on your device**.

- Thumbnails and full-resolution images are decoded by iOS into memory while you triage and discarded when you move on.
- Similar-photo detection uses Apple's on-device Vision framework. Feature prints are stored only inside Swoop's cache directory on your device.
- When you mark a photo for deletion and confirm, Swoop asks iOS to move that photo to the system "Recently Deleted" album using PhotoKit. iOS handles the actual deletion; Swoop never has direct access to your photo files.

## What Swoop stores on your device

- **App settings** (swipe directions, grouping preferences, etc.) in iOS UserDefaults.
- **Session state** (current index, pending decisions) so you can resume a triage session.
- **Similarity cache** (feature prints used to detect duplicates) in Swoop's private cache directory.

You can clear all of this by deleting the app.

## What Swoop sends off your device

**Nothing about your photos.** Swoop does not upload, transmit, or transmit metadata about your photos, videos, decisions, or browsing.

The only exception is optional anonymous diagnostics:

- **Crash reports and basic usage signals**, sent via TelemetryDeck if (and only if) crash reporting is enabled. These signals do not include any photo content, photo identifiers, file paths, or personally identifiable information. TelemetryDeck does not assign persistent user IDs and is GDPR-compliant. See: https://telemetrydeck.com/privacy/

If you do not want to send these signals, you can disable them in Settings → Privacy.

## Third parties

- **Apple PhotoKit** (system framework). Apple's privacy policy applies to underlying photo storage and deletion: https://www.apple.com/legal/privacy/
- **TelemetryDeck** (optional, for crash reporting). Privacy policy: https://telemetrydeck.com/privacy/

No other third parties.

## Children

Swoop has no age restrictions and does not knowingly collect data from anyone, including children.

## Changes

If we update this policy, we'll bump the "Last updated" date above and include a summary of the change in the next app release notes.

## Contact

Questions or concerns? Email **maxbergandersen@gmail.com**.

# LiftCapture Privacy Policy (beta)

**Effective date: October 7, 2026**

LiftCapture is a velocity-based training app for iPhone and Apple Watch,
currently in beta. Your training data lives on your devices. This page
says exactly when anything leaves them, where it goes, and how to stop it.

## At a glance

| What | Leaves your phone? | Where it goes |
|---|---|---|
| Workouts, sensor recordings, velocity results | Only through the options below | — |
| **Apple Health data** | **Never without your permission** | Only to the coach, and only if you allow it |
| A copy of your workouts | Yes, unless you turn off iCloud sync | Your own private iCloud. We can't read it |
| Beta metrics and sensor recordings | Only if you tap **Share motion data** (off until you do) | The app's iCloud database, for the developer |
| Coach chat, training-block design, import help | Only when you use those features | Our server (Cloudflare) and Anthropic's Claude |
| Update check | Yes: your app's build number only | Our server |

## Data stored on your device

Workouts you log (exercises, weights, reps, RPE), workout templates,
sensor recordings from your Apple Watch and iPhone (motion and heart
rate), and all velocity analysis results are stored locally on your
iPhone and Apple Watch. Velocity and rep analysis runs on your devices,
not on a server. Voice commands are recognized on your iPhone where it
supports this; otherwise Apple's speech recognition service handles them.

## Apple Health

With your permission (Apple's Health prompt), LiftCapture reads these
from Apple Health:

- your heart rate and distance during workouts;
- cardio workouts recorded by other apps, and their heart rate;
- VO2 max;
- body weight.

It saves the workout sessions and the body-weight entries you log to
Apple Health.

**Your Health data does not leave your phone without your consent.**
LiftCapture never includes it in beta telemetry, never copies it to
iCloud, and never uses it for advertising or data mining.

The one place it can be used off your phone is the coach. The first time
you open the coach chat or ask the coach to design a training block,
LiftCapture asks: **Share your Apple Health data with your coach?** That
means:

- your resting and recovery heart rate;
- VO2 max;
- heart rate and distance during workouts;
- workouts and body weight imported from Apple Health.

Nothing on this list is shared until you tap **Share Health data**, or
turn on **Share Apple Health data** in Settings › Coaching. If you choose
**Not now**, the coach works without it. You can change your answer at
any time with that setting.

This page describes LiftCapture as of 0.4.53 (build 92). Builds before
0.4.53 sent Health-derived lines without asking; the server now strips
them for those builds. It strips their body-weight lines too, because it
can't tell a Health weight from one typed in the app.

## Coach, training blocks and import help

These features send data to the LiftCapture server, which is hosted by
**Cloudflare**. The server passes it to **Anthropic**'s Claude models.
Both act as our service providers.

- **Coach chat** (Pro; currently limited to invited testers): each
  message, typed or asked aloud during a workout, sends your recent
  conversation (up to 24 messages) and a summary of your training. The
  summary covers:
  - your profile answers, including age and sex if you entered them;
  - lift estimates and trends;
  - recent sessions and ratings;
  - your preferences and your plan;
  - body weight you logged in the app.

  It includes Health data only if you allowed it (see Apple Health).
- **Training-block designs** (Pro; every TestFlight tester currently has
  Pro): a shorter summary plus your goal and progress is sent at these
  times:
  - when you start a block with a goal;
  - automatically, each block week;
  - when you tap Redesign.

  The same Health choice applies.
- **Import help** (anyone, only when you tap it): for a workout file the
  app doesn't recognize, the app sends the first 25 lines (column names
  plus up to 24 rows) and any app name you type, to work out the columns.

Anthropic receives this content but not your IP address or any account
identifier. Anthropic deletes it within 30 days, unless it must keep it
longer to enforce its usage policy or to comply with the law
([Anthropic's privacy center](https://privacy.claude.com/en/articles/7996866)).
Anthropic does not use it to train its models.

Our server does not store your messages, your summary or file rows. It
keeps:

- an account ID it creates for you, linked to Apple's identifier for
  your download of the app or, when that isn't available (as on
  TestFlight), to a random ID generated on your phone;
- your message allowance and purchase status, from the purchase records
  the app sends and Apple's purchase notifications. From these it keeps
  only your Pro end date and a record of each message pack you buy. When
  you buy, renew or get a refund, Apple sends our server a signed record
  of that purchase: the product, dates, price, store country and Apple's
  transaction IDs, but not your name, email or Apple ID.
- a usage log (time, feature, model, amount used);
- the import formats you used (identified by their column names, never
  rows) with the number of sets imported;
- recent coach replies, so a dropped answer can be resent. Replies over
  24 hours old are deleted when the next reply is stored, so your last
  replies stay until you use the coach chat again.

Apart from coach replies, these records have no automatic expiry today.
Server logs record request details. When a block design is corrected,
the log includes your account ID and the corrected lift loads and
strength estimates. Cloudflare keeps these logs for up to 7 days.
Cloudflare's record of each request also includes your approximate
location (such as your country) and may include your IP address.

## Update check

When you open LiftCapture, and at most hourly after that, the app asks
our server which TestFlight build is current, so it can tell you when
yours is out of date. The request carries your app's build number and no
account information. Like every request to our server, it appears in the
server logs described above.

## Beta metrics and sensor recordings (only if you opt in)

The first time you open LiftCapture, it asks whether to share motion
data. **Nothing is shared unless you tap Share motion data.** Choosing
**Not now** shares nothing, and the app works the same.

Tapping **Share motion data** turns on two things. Both are tagged with a
random identifier generated on your phone, not your name, email or Apple
ID.

1. **Derived workout metrics:**
   - exercise names, weights, reps and set types you log;
   - your RPE (effort) entries;
   - computed velocity metrics, rep timing and detected rep counts;
   - your rep-count feedback (correct/incorrect taps and corrected counts);
   - assisted and paused reps;
   - the app's suggestion for the set, and whether it was shown;
   - app version and workout timestamps.
2. **Raw sensor recordings:**
   - wrist motion and accelerometer data from your Apple Watch;
   - phone motion;
   - Apple Watch battery and event logs (for example, when the watch
     buzzed), with any event timed by your heart rate removed before
     upload.

In Settings you can keep the metrics on and turn the recordings off, or
turn both off; either stops further uploads.

- Sensor recordings upload automatically over Wi-Fi only; tapping
  **Sync now** sends them over any connection. Metrics upload over any
  connection.
- **Heart-rate recordings and anything from Apple Health are never part
  of this sharing.** Neither are your location, your name or email, or
  the free-text notes you write. The timing of some logged events can
  reflect heart-rate-based rest decisions; no heart-rate values leave the
  phone.

This data is stored in the app's public iCloud (CloudKit) database, which
requires you to be signed in to iCloud. Apple also attaches an
identifier for your iCloud account to each record. That identifier
doesn't reveal your name or email to us, but it keeps your records
linked even if the random identifier changes. No other identifier is
attached, and the random identifier is never sent to our server. The
database's current settings let other clients of the app's iCloud
container read these records too. We plan to restrict reading to the
developer. The developer downloads the data for analysis and uses it
only to improve rep detection, velocity estimation and app quality.

## Your iCloud

Unless you turn off **Sync workouts to my iCloud** in Settings,
LiftCapture copies these to your own private iCloud database:

- your workout summaries;
- per-set numbers;
- body-weight entries you type;
- exercise-name merges you make.

Notes are never synced, and neither is anything imported from Apple
Health. The developer cannot read your private iCloud data. The
LiftCapture website can show it to you in your browser after you sign in
with your Apple ID.

## What we don't do

- No sign-up or password in the app. Cloud features use the server
  account ID described above.
- No third-party analytics, advertising or tracking SDKs.
- No sale of your data, ever. Data reaches other companies only as
  described here:
  - Apple (iCloud, App Store, TestFlight, speech recognition);
  - Cloudflare (our server host);
  - Anthropic (the coach's AI model).

## TestFlight

Beta distribution uses Apple TestFlight. Apple's handling of TestFlight
tester information (such as your email invitation) is governed by
Apple's own privacy policy. Crash reports and feedback, including
screenshots, that you send through TestFlight are shared with the
developer.

## Data deletion

Telemetry cannot be traced to you by name. Contact the developer at the
address below for any of these:

- to delete telemetry linked to your identifier (shown as Anon ID in
  Settings › Beta debug);
- to delete your records on our server;
- with any privacy question.

Deleting the app removes the data stored on your devices. It does not
remove these:

- your private iCloud copies (delete those on your iPhone in Settings ›
  [your name] › iCloud › Storage or Manage Account Storage › LiftCapture
  › Delete Data from iCloud);
- telemetry already uploaded;
- our server records.

## Children

LiftCapture is not directed at children under 13.

## Changes

This policy may be updated during the beta; the effective date above
will change accordingly.

## Contact

Christopher Chin — chris.r.chin@gmail.com

# Liftometer Privacy Policy (beta)

**Effective date: November 23, 2026 (Liftometer 0.4.82, build 121)**

Liftometer is a velocity-based training app for iPhone and Apple Watch, currently in beta. Your training data lives
on your devices. This page says exactly when anything leaves them, where it goes, and how to stop it.

## At a glance

| What | Leaves your phone? | Where it goes |
|---|---|---|
| Workouts, sensor recordings, velocity results, programs | Only through the options below | — |
| **Apple Health data** | **Never without your permission** | Only to the coach, if you turn on **Coach data** and **Apple Health with the coach**; your heart rate for each set to the app's iCloud database, if you turn on **Heart rate with sets**; and, if you use the Points card, the times and length of workouts imported from Health to our server |
| **Your location** (outdoor walks, runs, rides) | **Never, except for directions:** when you search for a place, build a route or go off one, the places you search for or choose and your position go to Apple Maps | Used on your Watch and phone for distance and pace; Apple Maps only for a route's directions |
| A copy of your workouts | Yes, unless you turn off iCloud sync | Your own private iCloud. We can't read it |
| Beta metrics, app-usage metrics and sensor recordings | Only if you turn on **Share set and app-usage data** (off until you do) | The app's iCloud database, for the developer |
| Coach chat, training-block design, import help | Only when you use those features | Our server (Cloudflare) and Anthropic's Claude |
| Points for training | Yes, one claim per workout, if you use the Points card | Our server |
| Community boards | Only while you are a member of a community | Our server, and the board's other members see your handle, your rank and your score |
| Update check | Yes: your app's build number only | Our server |

## Data stored on your device

Workouts you log (exercises, weights, reps, RPE), workout templates, training blocks and programs (such as the
built-in Texas Method), sensor recordings from your Apple Watch and iPhone (motion and heart rate), and all velocity
analysis results are stored locally on your iPhone and Apple Watch. Velocity and rep analysis runs on your devices,
not on a server. Voice commands are recognized on your iPhone where it supports this; otherwise Apple's speech
recognition service handles them.

## Your location

If you pick an outdoor cardio type (Outdoor Walk, Run or Cycle), the app asks for your location once, before you
start. Your phone and your Watch each ask for location separately; a walk recorded by the Watch alone needs the
Watch's permission. Location is used only while that workout is recording, and while you build or pick a route (to know how far its start is), to measure distance and pace and to say the turns on a route. The app saves only the routes you build and name; it never records
where you went. Apart from a route's directions (below), it does not upload your location, never includes it in beta metrics, and never shows it to the coach.
The distance and pace it produces are saved with the workout on your devices and to Apple Health; they reach the coach
only under your Apple Health choice below. Indoor types never use location. If you decline, outdoor workouts record
without distance.

If you build a route, the app asks Apple Maps for directions. Apple receives the start, the places you search for or
choose and, when you go off the route or ask for directions to its start, your position at that moment, under Apple's
privacy policy; we receive nothing. The routes you build and name are saved on your phone only and are never
uploaded: never to Liftometer's servers or the chat coach, and never in beta metrics. A route you start without
naming it is kept only until that session ends. Delete a route any time under Routes; its line, turns and stops go
with it.

## Your phone's location in outdoor sessions

During an outdoor cardio session the app uses your phone's location to measure distance, including while the screen is off. Only the running total is kept. It goes to your Watch during the session and into the workout on this phone. Where you went is never stored, and your coordinates never reach us.

## Apple Health

With your permission (Apple's Health prompt, asked once), Liftometer reads these from Apple Health:

- your heart rate and distance during workouts;
- cardio workouts recorded by other apps, and their heart rate;
- VO2 max;
- body weight.

It saves the workout sessions and the body-weight entries you log to Apple Health.

**Your Health data does not leave your phone without your consent.** Liftometer never includes it in beta metrics
except for one item you turn on yourself, **Heart rate with sets** (below), never copies it to iCloud, and never uses
it for advertising or data mining.

Apart from **Heart rate with sets** (under Beta metrics below) and the times and length of Health workouts sent with a Points claim (see Points), the one place it can be used off your phone is the coach. The first time you open the coach chat or ask the coach to
design a training block, Liftometer asks: **Share your Apple Health data with your coach?** That means:

- your resting and recovery heart rate;
- VO2 max;
- heart rate and distance during workouts;
- workouts and body weight imported from Apple Health.

Nothing on this list is shared until you tap **Share Health data**, or turn on **Apple Health with the coach** in Settings › Privacy & security (shown under Coach data). That row shows under **Coach data** only while Coach data
is on; turning Coach data on doesn't turn it on. If you choose **Not now**, the coach works without it. You can change your answer at any time with that setting. That includes what the app works out from them: without your yes, the coach's
suggestions use only a weight you typed in the app or imported from a file. While that setting is off, the conversation from before you turned it off is not sent to the coach; it stays on your screen.

Builds before 0.4.53 sent Health-derived lines without asking; the server strips them for those builds. It strips
their body-weight lines too, because it can't tell a Health weight from one typed in the app.

## Saving distance to Apple Health

If you allow it, the app writes the distance of a phone-only outdoor session to Apple Health, and adds the difference to a Watch session when the phone measured more. You are asked from the summary after such a session, up to three times until you answer, and can change it in Settings › Health.

## Coach, training blocks and import help

These features send data to the Liftometer server, which is hosted by **Cloudflare**. The server passes it to
**Anthropic**'s Claude models. Both act as our service providers.

**Before your first message or block design, the app shows you this list and asks you to continue.** Your answer and
the version of this policy you saw are recorded on our server, so we can show that you agreed. You can withdraw by
turning off **Coach data** in Settings › Privacy & security, which turns off **Apple Health with the coach** too, or
only the Health part with its own row; turning off Coach data stops the coach until you agree again.

- **Coach chat** (Pro; currently limited to invited testers): each message, typed or asked aloud during a workout,
  sends your recent conversation (up to 24 messages) and a summary of your training. The summary covers:
  - your profile answers, including age and sex if you entered them;
  - lift estimates and trends;
  - recent sessions and ratings;
  - your preferences, your plan, the planned days still ahead in any block you're running (so a change can land
    on the right day), and whether you skipped or are making up a planned day;
  - body weight you logged in the app or imported from a file;
  - the routine and starting numbers you entered on the onboarding card, if you did: its split, days a week, each day's name and lifts, and your best recent and all-time sets as you typed them.

  It includes Health data only if you allowed it (see Apple Health). The app never attaches your location to a
  chat; what you type is up to you.
- **Training-block designs** (Pro; every TestFlight tester currently has Pro): a shorter summary plus your goal and
  progress is sent when you start a block with a goal, automatically each block week, and each time the block is designed again (for example when you tap Redesign, change its goal or its length, or switch coach).
  When you build or rebuild a block, your plan note (up to 280 characters), your answers to the block's optional
  questions and the training days you chose for each lift go with it, so the coach can shape the block's weeks. The
  same Health choice applies.
- **Import help** (anyone, only when you tap it): for a workout file the app doesn't recognize, the app sends the
  first 25 lines (column names plus up to 24 rows) and any app name you type, to work out the columns.

Anthropic receives this content but not your IP address or any account identifier. Anthropic deletes it within 30
days, unless it must keep it longer to enforce its usage policy or to comply with the law
([Anthropic's privacy center](https://privacy.claude.com/en/articles/7996866)). Anthropic does not use it to train
its models.

Our server does not store your messages, your plan note or file rows, and of your summary only what is kept with a coach reply that proposed a plan change (below). It keeps:

- an account ID it creates for you, linked to Apple's identifier for your download of the app or, when that isn't
  available (as on TestFlight), to a random ID generated on your phone;
- your message allowance and purchase status, from the purchase records the app sends and Apple's purchase
  notifications. From these it keeps only your Pro end date and a record of each message pack you buy. When you buy,
  renew or get a refund, Apple sends our server a signed record of that purchase: the product, dates, price, store
  country and Apple's transaction IDs, but not your name, email or Apple ID;
- a usage log under your account ID: time, feature, model, amount used and its cost, how long the request took, your app's build number, whether the request came from
  a test build, and whether the server retried the model and which of its checks asked for the retry (never what was said). For a block design, the row also
  keeps the design itself (for each week, each lift's name with its sets, reps, percentage of its estimated max and effort, and the loads the coach set), so a wrong design can be
  traced, but never your note. A lift you named yourself appears under the name you gave it;
- the import formats you used (identified by their column names, never rows) with the number of sets imported;
- a shared list of file formats: a format's column names and the app name given for it, not linked to you, so the next person with the same file gets its mapping and sees that app name. It is not deleted with your account;
- recent coach replies, so a dropped answer can be resent, each with its time, the model, the amount used and how the reply ended. A reply can quote what you wrote. A reply that proposed a plan change is also kept with: the change as the server checked and corrected it; for each lift it touches, the lift's strength estimate, whether that estimate comes from bar speed or effort ratings, and what the app itself suggested for the lift (reduce, hold or step up); the week of your block and which version of its plan the change was for; your app's build and the version of the coach's instructions; whether that turn was about pain or a warning sign; and whether Health data was allowed for it. If the server's own checks turned a proposed change down, the names of those checks are kept. Replies over 24 hours old are deleted when the next reply is stored, so your last replies stay until you use the coach chat again.

Apart from coach replies, these records have no automatic expiry today. They are deleted when you delete your
account, except the usage log and the shared list of file formats (see Data deletion). Server logs record request details. When a block design is corrected, the log
includes your account ID and the corrected lift loads and strength estimates. Cloudflare keeps these logs for up to
7 days. Cloudflare's record of each request also includes your approximate location (such as your country) and may
include your IP address.

**Delete my coaching data** (Settings › Coaching) erases the stored coach replies and unlinks your usage rows from
you, with your account ID on them replaced by the word "deleted" and any block design removed from them, without
deleting the account; the app clears its local chat too. Your month's message count is kept, so deleting cannot
reset your allowance.

If a chat ever freezes, Settings › Diagnostics › **Copy this chat as JSON** puts that conversation on your clipboard
for you to send us. Nothing is sent unless you send it. From a chat's menu you can copy a message, or export a chat or all your chats as a text file through the share sheet. The file holds the words you and the coach exchanged and each card's visible lines, never the coach's summary of your training. Nothing leaves the phone unless you share it.

## What the coach sees

For each lift, the coach also sees the next plate step the app would offer, the effort you rated your last session's working sets at, and your program's current set scheme: sets, reps, step-down rung and stall count. These come from your own log, like everything else the coach sees.

## Points

If you use the Points card, the app sends our server one claim for each workout: a session ID, start and end times,
how many working sets you did and how many the Watch captured, cardio minutes, the local date, your weekly sessions
target, which planned block days were done, and whether the session was logged in the app or imported. It also
carries a proof of the claim made from the app's own install id, not the id itself, so a resent claim is counted once.
While a
training block runs, it also carries, for each lift a running block judges that week, how much of its planned work you
did (a share from 0 to 1), a code for the block week and, once the week has one, the day it ends (a block run by workouts gets its end day
when its week closes). Each lift is sent as a short code that identifies the lift
(bench press, squat, and so on), not the name as you typed it. No loads, reps, heart rate or notes. The server keeps
the counts, the date, its decision and, while a block runs, each judged lift's code and share. It keeps the session ID, which is made from the workout's start time; it does not keep the end time. The server checks the claim is plausible and writes your
points; claims it rejects are kept with the reason, so we can see why. Points are tied to your server account, not
to the anonymous metrics ID. They are deleted with your account.

## Communities

Joining a community needs an invite link from its host. Before you join, the app shows what the board will show. While
you are a member, our server keeps your membership (your competition handle, or "anonymous" if you choose that), and
each week a row of counts: sessions done against your target, planned block sets against sets done, and sets total
against sets the Watch captured. The app suggests a handle, a word and an animal picked on your phone; only the handle
you keep reaches the server. The board ranks those ratios, never the weight you lift. Other members see your
handle and your place; the host sees the member count and the board, nothing else. Leave with one tap in the
community's screen; the row is marked ended and kept until you delete your account. Invites you create are kept
with their code and use count, and revoked invites are kept the same way. All of it is deleted with your account; a community you host is closed for its
members, and its name and events stay on the server, no longer linked to you.

## Update check

When you open Liftometer, and at most hourly after that, the app asks our server which TestFlight build is current,
so it can tell you when yours is out of date. The request carries your app's build number and no account
information. Like every request to our server, it appears in the server logs described above.

## Beta metrics, app-usage metrics and sensor recordings (only if you opt in)

Every sharing choice is on one card, **Privacy & security**: the first time you open Liftometer it is shown to you,
and it stays in Settings › Privacy & security. Each row says in one line what it shares: **Share set and app-usage data**, **Share body-weight and sex bands** (under it, and only with it on), **Coach data**, **Apple Health with the coach** (shown under Coach data while it is on), **iCloud sync**, **Apple Health** and **Location** (these two show what iOS has allowed, with
a button to ask or to open iPhone Settings; the app can't switch them itself), and, under **Help improve velocity
detection**, **Wrist motion recordings** and **Heart rate with sets**. **Nothing is shared with us until you turn a row on.**
Tapping **Done** without turning anything on shares nothing with us, and the app works the same. Your own iCloud
keeps a private copy of your workouts unless you turn **iCloud sync** off.

At the bottom of the card, under every row's line, **Allow all** turns on every row the card shows at that moment, including the bands and the two velocity-detection rows (the bands stay off if you said no to them before), and records your agreement to coach data sharing at the version the card links to. It turns on **Apple Health with the coach** only if that row was showing at the tap, which needs Coach data already on or waiting for a connection; otherwise that row appears under Coach data afterwards and stays off until you turn it on. **Allow all** then
asks iOS for Apple Health and Location, once each, if you haven't answered those yet; iOS's own prompts decide what is
allowed. Without a connection, the coach row waits and is sent when you're next online; the coach stays off until then.
Every row can be turned off again on its own, with no confirmation, in Settings › Privacy & security.

Turning **Share set and app-usage data** on shares four things; the bands in item 1, and items 3 and 4, also need their own rows turned on. All are tagged with a random identifier generated on your phone, not your name,
email or Apple ID.

1. **Derived workout metrics:**
   - exercise names, weights, reps and set types you log;
   - your RPE (effort) entries;
   - the set's number in the workout;
   - computed velocity metrics, rep timing and detected rep counts;
   - for each set's speed, which version of the analysis rules measured it;
   - your answer to the timing recheck, if you gave one;
   - your rep-count feedback (correct/incorrect taps and corrected counts);
   - assisted and paused reps;
   - the app's suggestion for the set, and whether it was shown;
   - the reps, load and effort the set was planned at before you started it, and whether you attempted one more rep and failed it;
   - the rest you took before each set, the rest the plan asked for, what ended the rest (the clock, your heart rate,
     or you), and whether heart-rate rest was on;
   - only if you turn on **Share body-weight and sex bands** (off until you do), your body-weight band and sex, as bands, never the numbers: a 10 kg band such as "70-79 kg" (the ends read
     "under 50 kg" and "130 kg and over") from the latest body weight you entered in the app or imported from a file
     (never one from Apple Health) and the sex on your profile, each "unsaid" if you haven't entered it;
   - app version and workout timestamps.
2. **App-usage metrics:** how long the app's own steps take and which screens and buttons were used, as event names
   from a fixed list with their times, durations, counts and a few fixed words, plus the build number, your access level (tester, invited tester or developer) and a random per-launch ID.
   Never any text you typed, no lift names, no loads, no RPE, no heart rate, and nothing from Apple Health. Up to 200
   events per launch.
3. **Wrist motion recordings** (the **Wrist motion recordings** row):
   - wrist motion and accelerometer data from your Apple Watch;
   - phone motion;
   - Apple Watch battery and event logs (for example, when the watch buzzed), with any event timed by your heart rate
     removed before upload.

4. **Heart rate with sets** (the **Heart rate with sets** row): your heart rate for each set, as its average and peak,
   or, if you choose **Zone only**, just its zone (Easy, Steady or Hard, against your max heart rate); in either form,
   also how long your heart rate took to settle after the set. Your Apple Watch measures it during the workout, so it
   is Apple Health data; this row is the one way any of it enters the shared data, and nothing else from Apple Health
   ever does, apart from the rest timing in item 1, which says only whether your heart rate ended a rest, never a
   value.

**Help improve velocity detection.** The card asks for the last two separately, under their own heading, because they
are what we use to make bar-speed detection better: the raw wrist motion shows where each rep starts and ends, and
heart rate shows how hard a set was against its speed. Both are off until you turn them on, each on its own: turning
one on never turns the other on. Both need **Share set and app-usage data** on, because they go under the same random
identifier.

In Settings › Privacy & security you can keep the metrics on and turn either of the last two off, or turn everything
off; either stops further uploads.

Turning **Heart rate with sets** off stops further uploads. **Remove shared heart rate** also clears it from the sets you already shared, usually within a day. Turning **Share body-weight and sex bands** off stops further uploads. **Remove shared bands** also clears them from the sets you already shared, usually within a day.

- Sensor recordings upload automatically over Wi-Fi only; tapping **Sync now** sends them over any connection.
  Metrics upload over any connection.
- **Your location, heart-rate recordings and anything else from Apple Health are never part of this sharing,** nor
  are your name or email, or the free-text notes you write. The only heart-rate values that leave the phone are each
  set's, under **Heart rate with sets**. The timing of some logged events can reflect heart-rate-based rest decisions.

This data is stored in the app's public iCloud (CloudKit) database, which requires you to be signed in to iCloud.
Apple also attaches an identifier for your iCloud account to each record. That identifier doesn't reveal your name
or email to us, but it keeps your records linked even if the random identifier changes. No other identifier is
attached, and the random identifier is never sent to our server. Other users of the app can't read these records; only the developer can. The developer downloads the data for analysis and uses it only to improve rep detection, velocity estimation and app quality.

## Sessions closed for you

A workout left open with no sets for four hours is closed the next time you open the app or start a workout, on the phone or the Watch, as if you had tapped Finish. Its sets count toward your history. If you share set data, they upload as a finished workout's would. A Health workout is written only if you had already allowed that.

## Your iCloud

Unless you turn off **iCloud sync** in Settings › Privacy & security, Liftometer copies these to your own private iCloud
database:

- your workout summaries, including workouts you import from a file and the "Starting numbers" workout made from numbers you type on the onboarding card;
- per-set numbers;
- body-weight entries you type or import from a file;
- exercise-name merges you make.

Notes are never synced, and neither is anything imported from Apple Health. The developer cannot read your private
iCloud data. The Liftometer website can show it to you in your browser after you sign in with your Apple ID.

## What we don't do

- No password in the app. Cloud features use the server account ID described above.
- No third-party analytics, advertising or tracking SDKs.
- No sale of your data, ever. Data reaches other companies only as described here:
  - Apple (iCloud, App Store, TestFlight, speech recognition, Health, Maps for route directions);
  - Cloudflare (our server host);
  - Anthropic (the coach's AI model).

## TestFlight

Beta distribution uses Apple TestFlight. Apple's handling of TestFlight tester information (such as your email
invitation) is governed by Apple's own privacy policy. Crash reports and feedback, including screenshots, that you
send through TestFlight are shared with the developer.

## Data deletion

**Deleting a workout:** If you delete a workout, it is gone from your phone and your plan. The copy you already
shared for the beta stays on the server marked deleted and is left out of every analysis; it is not erased.
The app keeps trying for a few days; if it can't reach iCloud by then, it tells you and you can retry.
Restoring it from Recently Deleted within 30 days takes the mark off. The app keeps trying for a few days; if it
cannot reach iCloud by then, the shared copy stays marked deleted.
If a set's place in a workout changes, or you uncheck or remove a set, its earlier shared copy is marked deleted.
Recordings of a deleted workout that are still on your Watch are not uploaded while it is deleted. Once the workout is
gone for good, the Watch deletes them when it next reaches your phone, or the phone deletes them with its other old
recordings.

**Delete your account in the app:** Settings › Account › **Delete account…** (or **Delete account and data** in Settings ›
Privacy & security), then confirm **Delete everything?**.
Your account is gone from our server at once. This deletes, at once:

- your account ID and every identifier linked to it (Apple's identifier for your download, the random ID from your
  phone);
- your points, and the claims behind them;
- your community memberships, the weekly counts the boards use, and the invites you created. A community you host is
  closed for its members; its name and events stay on the server, no longer linked to you;
- the import formats you confirmed.

The rest follows, usually within minutes, and is retried until done:

- your message allowance, purchase status and message-pack records;
- your consent record and your coach history: the recent coach replies kept for resending.

If the app closes before the deletion has finished, the app continues it the next time you open it with a connection. If it
could not confirm the deletion with our server within seven days, or our server does not accept the repeated
request, the app stops and tells you, so you can start the deletion again.

**What we keep:** the usage log rows stay for our cost accounting, with what is listed for the usage log above, but
with your account ID replaced by the word "deleted" and any block design removed from them, so they no longer link
to you or to anything else we hold. The shared list of file formats stays too; it was never linked to you. The log also gains one entry, not linked to you, recording that an account was deleted.

**After a deletion** the server keeps your former account ID and the time of the deletion, for one purpose: to refuse the session your phone
already held (a session lasts at most 30 minutes). That ID stops being used after 31 minutes and is removed at the
next cleanup.

Purchases are Apple's: deleting your account doesn't cancel a subscription (cancel it in iPhone Settings › Apple ID ›
Subscriptions), and Pro comes back on this phone from your App Store purchase.

Two options on the same screen, both off unless you turn them on:

- **Also erase my workouts on this phone** deletes every workout on the phone with its recordings, their copies in your private iCloud, Recently Deleted, the app's own logs of those workouts (rests, check-off lines, the weekly review) and any training-data export the app still holds. Recordings of those workouts that were not uploaded yet are not sent; an upload already under way at that moment can finish. What stays on this phone: what the app has learned from your workouts (such as your usual rep speed, effort ratings, heart-rate recovery and your rep-count corrections), the awards you earned, the starting numbers you entered, your block plan with its records, your coach chats, templates, body weights, settings and the app's diagnostic notes. Deleting the app removes them. Without this option your workouts stay on the phone.
- **Also delete the anonymous data I shared** deletes the beta metrics, app-usage metrics and sensor recordings this
  phone uploaded under its random identifier, and turns sharing off. Copies the developer already downloaded for
  analysis are not reached that way: contact the developer to have them deleted too.

Erasing all workouts on this phone doesn't mark the copies you already shared. Deleting your account with "Also
delete the anonymous data I shared" turned on deletes them.

A file you have shared or saved outside the app (a training-data export, a chat export, a recording, a share card) is
a copy the app can no longer reach; delete it where you saved it.

You can also contact the developer at the address below for any of these, or with any privacy question.

Deleting the app removes the data stored on your devices. It does not remove your server account (delete it in the
app first), metrics already uploaded, or your private iCloud copies (delete those on your iPhone in Settings › [your
name] › iCloud › Storage or Manage Account Storage › Liftometer › Delete Data from iCloud).

## Children

Liftometer is not directed at children under 13.

## Changes

This policy may be updated during the beta; the effective date above will change accordingly.

## Contact

Christopher Chin — chris.r.chin@gmail.com


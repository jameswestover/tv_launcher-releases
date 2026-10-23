# Westy releases

Signed builds of the Westy TV launcher. Boxes check here once a day and
update themselves when nobody is using the TV. New builds start as betas
(pre-releases) and become releases once they've been tested. Newest first.

## v0.12.4 · 2026-10-23
- **Settings:** the on-screen back arrow is gone; press Back on the remote. The menu now
  wraps around: up from the top goes to the bottom, and down from the bottom to the top.
- **Power** is one button, **Turn off or restart**, which opens the box's power menu,
  instead of two buttons that both ended up there anyway.
- **Update** in an app's hold-OK menu now stays on Home: Westy checks the app's Play Store
  page behind the scenes and either starts the update (the tile greys out with a spinning
  ring until it's installed) or shows "Up to date" under the tile.
- After a force quit or update, focus comes back to that app instead of the first one.

## v0.12.3 · 2026-10-23
- **The remote always works during a force quit.** Version 0.12.2 ignored it for those few
  seconds; now only the Home button does anything special (it cancels).
- Behind the scenes: Westy picks its own download by name, so the update helper can later
  be published alongside each release.

## v0.12.2 · 2026-10-23
- **Update an app:** hold OK on it on Home and choose **Update**. It opens the app's Play
  Store page, which has an Update button when there's one.
- **Settings > Apps > App updates** explains where to choose automatic or manual app
  updates in the Play Store, with a button to open it.
- **Fixed:** force quit could leave the screen frozen at the end. It now always finishes
  within a few seconds, and the Home button cancels it straight away.

## v0.12.1 · 2026-10-23
- **Force quit** no longer flashes a full-screen "Closing…" message. The app's tile greys out
  and a little ring fills in on it, like an app updating on a phone, then the tile turns back
  to normal when it's done.
- **Fixed:** the Westy logo could play again when coming back from Google's screens (like
  Manage accounts) after an update. It now plays once per update or restart.

## v0.12.0 · 2026-10-23
- **Settings is tidier:**
  - The menu is in groups: Home, the TV, connections, updates, then Power.
  - **Screensaver & sleep** is now one page, with both choices side by side.
  - "Set up TV control" is now just **TV control**.
  - **Updates** is shorter, and says when you're on the beta channel.
  - **Power** has its two buttons side by side.

## v0.11.3 · 2026-10-23
- **Force quit** now happens behind a "Closing …" screen, instead of showing Android's
  App info screen while Westy presses its buttons.
- **Force quit on an app that isn't open** goes straight back to Home, instead of stopping on
  Android's App info screen.
- **Settings > Developer:**
  - The channel choice now just says **Release** or **Beta**.
  - A **Check for updates** button checks on that channel and refreshes the version list.
  - Picking a beta in the list offers **Make public**, which makes it the version every
    box gets.

## v0.11.2 · 2026-10-23
- **New name: Westy.**
- **Updates no longer flash the last app you used** while Westy restarts. A plain "Installing
  update" screen covers the gap instead. Needs the small "Westy updater" helper app, which
  setup-box.sh now installs.
- **Settings > Developer** marks the version every box gets as **Public**, next to the betas.

## v0.11.1 · 2026-10-23
- **Hold OK on an app** now opens a small dropdown right under it, like a right-click menu,
  instead of a box in the middle of the screen.
- **Settings > Updates** shows exactly when it last checked, for example "checked at
  Oct 23, 5:10 AM".

## v0.11.0 · 2026-10-23
- **New name: WestyBox.**
- **Hold OK on an app** on Home for a menu:
  - **Force quit** closes an app that's stuck, then comes back to Home.
  - **Move** lets you slide the app left or right with the arrows; press OK to drop it, or
    Back to leave it where it was.
- **Settings > Apps** has a new choice, **Order on Home**: **Most watched first** (as before)
  or **In my order**. Moving an app switches to "In my order".
- **Restarting the box** stays on Home instead of reopening the last app.
- **Sleep after** now lists the time the box was already set to (Google's default is
  20 minutes), so the current choice is always ticked.

## v0.10.0 · 2026-10-23
- **Settings > Developer** (only on the developer's own box): try new versions as betas
  before everyone else gets them, and go back to any earlier version.
- New versions now reach the other boxes only after they've been tested.

## v0.9.1 · 2026-10-23
- **After an update** you asked for, Westy-ku restarts with its logo animation and
  "Updated to version …" underneath, then lands on Home. If an update fails, Settings >
  Updates opens to show why.

## v0.9.0 · 2026-10-23
- **Installing an update** now shows an "Installing…" screen, then Westy-ku restarts and
  opens Settings > Updates saying "Updated to version …" (or why it didn't install).
- **Google account:** just one button now, **Manage accounts**.
- **Back from Google's screens** (Wi-Fi, accounts and so on) now always returns to Westy-ku,
  instead of sometimes to another Google screen opened earlier.

## v0.8.0 · 2026-10-23
- **Google account:** new Settings section to switch, add or remove the Google account the
  box and Play Store use (it opens Google's own account screens).
- **Buttons all look the same:** see-through with an outline, turning solid white when the
  remote is on them. The white button is always the one OK presses.
- **Settings:** moving right from the menu always lands on the first option in a section
  (for example "Check for updates", not the Google system button).
- **After an update:** Westy-ku starts straight back up on Home, and turning the TV back on
  shows Home instead of the last app.

## v0.7.0 · 2026-10-23
- **Install updates automatically** (Settings > Updates, on by default). Updates install by
  themselves whenever nobody is using the TV: after Home sits untouched for 3 minutes, once
  the screensaver has been on for 2 minutes, or when the TV turns off. Never while an app
  like Netflix is open. Turn it off to only install when you choose.
- **Check for updates** in Settings > Updates asks "Install it now?" when it finds one, and
  the button becomes **Install update**: press it and Westy-ku restarts on the new version
  within seconds.

## v0.6.2 · 2026-10-23
- **Settings:** pressing Back inside a section (like Apps or Network) now returns to the
  Settings menu instead of to Home. Back from the menu still goes Home.

## v0.6.1 · 2026-10-23
- **Remote buttons:** pressing Back while choosing an app for a button, or while waiting
  for a button press, now goes back to the list of buttons instead of to Home.
- **Waking up:** turning the TV back on always shows Westy-ku's Home, instead of sometimes
  returning to the last app that was open.

## v0.6.0 · 2026-10-23
- **Remote buttons:** new Settings section to choose which app each app button on the
  remote opens. Choose "Add a button", press the button on the remote, then pick the app.
  Pick "Nothing" to turn a button off again. The buttons work from anywhere, even inside
  other apps.

## v0.5.0 · 2026-10-23
- **Settings reordered:** Apps, Set up TV control, Screensaver after, Sleep after, Network,
  Updates, Power.
- **About removed:** the Westy-ku version now shows on the Updates row.

## v0.4.0 · 2026-10-23
The first published release.
- **Home:** your apps, most watched first, six to a row (more wrap into centered rows), with
  the Westy-ku name, a clock, a "No internet" warning and a gear for Settings.
- **Startup:** "Westy-ku" bounces in letter by letter after the box boots.
- **Settings:**
  - **Apps:** tick any installed app to show it on Home; "Get more apps" opens the Play Store.
  - **Network:** connection type, signal, IP address, router and DNS.
  - **Set up TV control:** a music test to make sure the remote controls the TV.
  - **Screensaver after** and **Sleep after** timers.
  - **Updates:** checks for Westy-ku updates, and opens Google's system update screen.
  - **Power:** turn the box and TV off, or open the power menu to restart.
- **Screensaver:** public-domain landscape paintings, slowly crossfading and panning.
- **Updates itself:** checks once a day and installs when the TV turns off.

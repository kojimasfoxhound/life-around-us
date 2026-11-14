# Patch notes

## v1.5

To update, download the new **Life-Around-Us-Build-Kit.zip** from [Releases](../../releases/latest), extract it and build again with your v1.00 PKG folder. Then install the new `Life Around Us Setup.exe` over the old one.

### Improved
- **Start-up screen.** The splash now says the app covers **over 110 cities** (it said over 80).

### Known issue
- The local time next to each city shows the time when the app started or last refreshed (every 3 hours), not the minute you are looking at it. A fix is being worked on.

---

## v1.4

To update, download the new **Life-Around-Us-Build-Kit.zip** from [Releases](../../releases/latest), extract it and build again with your v1.00 PKG folder. Then install the new `Life Around Us Setup.exe` over the old one. The build now also downloads NASA's Earth images (about 270 MB, once).

### New
- **Your own music.** Make a folder called **Music** on your Desktop and put songs in it (subfolders too): MP3, M4A/AAC, Apple Lossless, FLAC, WAV or WMA. They play after the soundtrack.
  - **Music > My Music** lists your songs (up to 50). Pick one to play it and carry on through your songs, or choose **Play All My Songs**.
  - **Music > Original Soundtrack** goes back to the original loop (ThemeSong06, ThemeSong03, then the rest).
  - Your choice is remembered. A file that cannot play is skipped.
- **A NASA Earth that follows the month.** The day side uses NASA's Blue Marble for the current month: snow across the north in winter, green land in summer, in the app's own colours.
- **Newer night lights with a glow.** NASA's Black Marble 2016 replaces the app's city lights from around 2000: today's cities, roads and coastlines, with a soft halo round the big ones.
- **The Milky Way** behind the twinkling stars.
- **7 more live webcams:** London, Sydney, Toronto, Las Vegas, Wellington, Salt Lake City and Boise (13 in all).
- **Miami, Kingston and Santo Domingo** (133 cities). Havana is removed.

### Improved
- **Cleaner menus.** The PlayStation button shapes next to the "Life" logo in the menus are gone.
- To go back to the original Earth, set `LWP_EARTH=classic`; to turn off the Milky Way, `LWP_MILKYWAY=0`.

### Fixed
- **No black ring round the Earth.** Zoomed out, the night side of the atmosphere no longer hides the stars behind it as a dark border.

---

## v1.3

To update, download the new **Life-Around-Us-Build-Kit.zip** from [Releases](../../releases/latest), extract it and build again with your v1.00 PKG folder. Then install the new `Life Around Us Setup.exe` over the old one.

### New
- **Hurricanes, typhoons and cyclones.** Every **Category 4 or 5** storm, in any ocean, appears on the globe at its last reported position:
  - a blue swirl marker with its name, for example "Typhoon Cempaka"
  - its category and wind speed (km/h, or mph when you use Fahrenheit)
  - a panel with its position, when it was reported and the nearest country
  - Data comes from GDACS (NOAA and JTWC advisories). It is checked at start-up and every 3 hours, and the auto tour reaches storms early.
- **The International Space Station, live.** A marker follows the real ISS across the globe second by second, with a NASA photo and its altitude. Its path for the next few hours is downloaded with each refresh, so it keeps moving even between refreshes.
- **Earthquake rumble.** When the globe arrives at a new earthquake, the controller rumbles: 2 pulses below M6.5, 3 below M7.5 and 4 above that, stronger for bigger quakes. Each quake rumbles only once. Works with DualSense and DualShock 4 (USB or Bluetooth) and Xbox controllers. Set `LWP_RUMBLE=0` to turn it off.

---

## v1.2

To update, download the new **Life-Around-Us-Build-Kit.zip** from [Releases](../../releases/latest), extract it and build again with your v1.00 PKG folder. Then install the new `Life Around Us Setup.exe` over the old one.

### New
- **Live webcams.** Six cities show a current camera picture of the city, marked **LIVE**, instead of a photo: **Hong Kong, Chicago, Vienna, Berlin, Seattle and Paris**. If a camera is offline or its picture is old, the city's normal photo is shown.
- **Live refresh every 3 hours.** News, weather, webcams and earthquakes update by themselves while the app runs. The refresh only happens when nobody has touched the controller for 10 seconds (or the auto tour is running): the app reloads in a couple of seconds and the music carries on where it left off.
- **Breaking news first.** Headlines marked "Breaking", "Just in", "Live updates", "Developing" or "Urgent" go to the top of each city's news. News is from the last 24 hours.
- **The globe flies to new earthquakes.** When a new earthquake comes in, the camera goes straight to it and stays for 10 seconds so you can read about it, then the auto tour carries on.

### Changed
- **Earthquakes: magnitude 6.0 or stronger** (was 5.0, which happens many times a day), from the **last 3 hours** (was 1 hour), matching the refresh.
- **The auto tour visits every city once** before any city comes round again.
- **Music order.** At start-up ThemeSong06 plays, then ThemeSong03, then the rest of the soundtrack. After the last track it starts again from ThemeSong06.

### Fixed
- **City clocks no longer stop.** After running for many hours, the local time next to some cities could stop updating. Every label now stays matched to its city, and a label that was missed is found again and corrected.
- **No more black screensaver.** The PS3 screensaver, and its "Music is currently disabled" message that covered the globe, are turned off. The auto tour takes its place.
- **Logs from the previous run are kept** as `run.prev.log` and `update.prev.log` in the app folder, which helps if you report a problem.

---

## v1.1

To update, download the new **Life-Around-Us-Build-Kit.zip** from [Releases](../../releases/latest), extract it and build again with your v1.00 PKG folder. Then install the new `Life Around Us Setup.exe` over the old one. Your settings are reset to the defaults.

### New
- **Full screen.** Life Around Us now opens full screen. Press **Alt+Enter** or **F11** to switch between full screen and a window. The mouse pointer hides in full screen.
- **Earthquakes.** Every magnitude **5.0 or stronger** earthquake from the **last hour** shows up on the globe:
  - a red marker labelled "M5.x Earthquake" with the location
  - a panel with magnitude, depth and the time it struck (your local time)
  - a picture with the magnitude
  - Data comes from the U.S. Geological Survey and is checked every time you open the app.
- **Celsius or Fahrenheit.** The options menu now has **Settings > Weather > Temperature > Celsius / Fahrenheit**. It switches every city at once, the live clocks keep running, and your choice is remembered.
- **13 new cities (131 in all):**
  - **Middle East and Asia:** Aleppo, Baghdad, Kathmandu, Tashkent
  - **Somalia:** Bosaso, Hargeisa
  - **Spread across the globe:** Reykjavík, Honolulu, Havana, Brasília, Jakarta, Malé, Perth

### Improved
- **Smoother globe edges.** Edge anti-aliasing smooths the jagged rim of the Earth and the city dots. Text and menus stay sharp.
- **Faster auto tour.** Leave the controller alone for **10 seconds** (was 15) and the camera starts flying from city to city. Touch anything to take over.
- **Options menu.** The top menu now shows **Settings** and **Music**.
- **City photos.** Each city shows a single photo of the city. Collages, flags, maps, satellite images and old paintings are no longer picked.

### Fixed
- **Alt+Enter no longer opens the main menu.** While Alt is held, the keyboard doesn't press controller buttons, so Alt+Enter, Alt+Tab and Alt+F4 don't trigger START.
- **Music stays off when you turn it off.** If you choose Music > Disabled, the music no longer starts 30 seconds later anyway.
- **Build kit:** a clear message if the kit is run from a temporary folder (for example, straight from the zip).
- **Build kit:** making the setup no longer fails when the kit's folder name has spaces in it.

---

## v1.0

First release: a native Windows PC build of Life with PlayStation v1.00, built from your own copy with the build kit. Highlights:
- Native x86-64 program using DirectX 12, at a smooth 60 fps (1440p on stronger GPUs, 1080p on weaker ones)
- Live news, weather and city photos working again, refreshed each time you open the app
- 118 cities with live local time, whole-degree temperatures and clouds and cities shown together
- Twinkling stars, brighter city lights and a sharper Earth
- Music menu with named tracks and moods, an ocean-wave ambience and ThemeSong06
- "Your City" card with your local weather and time
- No PlayStation Network or sign-in needed
- DualSense, DualShock 4, Xbox controllers and keyboard
- One-click installer and the "Life Around Us" branding

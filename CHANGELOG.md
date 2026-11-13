# Patch notes

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

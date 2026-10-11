# Rodrigo Rio-Tinto

**Software Engineer — Backend, Full-Stack & Product Engineering**

I build software across the whole stack of connected products: backend APIs and
data pipelines, mobile apps, polished web front ends, interactive 3D, and the
tooling that ties them to real hardware. My recent work spans a Node.js/PostgreSQL
ingestion service, a React Native client, an encrypted pilot-activation system,
and a WebGL product experience for a combat-sports wearable.

---

## Technical Focus

| Area | Tools |
| --- | --- |
| **Backend** | Node.js, Express, REST API design, request validation, CORS |
| **Data** | PostgreSQL (schema design, relational modelling, time-series readings), Supabase |
| **Mobile** | React Native, Expo, React Navigation, Bluetooth Low Energy |
| **Web & Front End** | JavaScript (ES modules), HTML/CSS, design systems, self-hosted typography, responsive layout |
| **3D & Graphics** | Three.js / WebGL, procedural geometry, PBR materials, OBJ/MTL asset pipelines |
| **Security** | AES-GCM and PBKDF2 (Web Crypto), TLS certificate tooling, token-based access |
| **Hardware Integration** | Bluetooth Low Energy, IMU sensor data, firmware-to-cloud data flow |
| **Tooling** | Git, Node.js CLIs, Python, shell scripting |

---

## Selected Work

### Impkt — Combat-Sports Wearable Platform
[`TlNT0/Impkt`](https://github.com/TlNT0/Impkt)

Product site and pilot programme for a wearable built around a 9-axis IMU
sampling at 1000 Hz. I handle the web presence, the pilot activation flow, and
the pipeline that captures per-punch motion data (gyro, accelerometer,
orientation) from the band.

- Built a pilot activation service where each athlete redeems a one-time code.
  Pilot records are stored **encrypted** (AES-GCM with PBKDF2 key derivation),
  so the data file is safe to publish.
- Wrote a dependency-free Node.js CLI to issue, list, and manage pilot codes.
- Added a shared leaderboard backed by Supabase and keyed by pilot code.
- Built an interactive Three.js experience for the product: a scroll-driven PCB
  model with procedural yarn geometry and physically based materials, plus a
  custom asset-packing script.
- Designed the site and pilot pages around a single design system with
  self-hosted fonts and no framework dependencies.
- Maintained print-ready collateral as reproducible source (HTML to PDF via
  headless Chrome) rather than one-off files.

### Camelot — Environmental Monitoring Backend
*Private repository*

An air-quality telemetry system: a BLE-connected mobile client and a REST
backend that ingests and serves sensor data.

- Designed a PostgreSQL schema covering devices, time-stamped readings, and
  generated advice, with 14 measured quantities per reading (CO, CO₂, NO₂, NH₃,
  CH₄, H₂, PM10, humidity, pressure, temperature, light, and others).
- Built an Express API for reading ingestion, per-device history, device
  listing, and advice retrieval, with IP-based geolocation for each device.
- Built the companion React Native (Expo) app with dashboard, per-metric detail,
  and environment views over Bluetooth Low Energy.

### Secure Local Proxy Tooling
Worked with a private certificate authority and a TLS-intercepting proxy for
local debugging of device and app traffic, which gave me hands-on experience
with certificate chains, SANs, and trust configuration.

---

## What I Bring to a Team

- **End-to-end ownership.** I have taken features from the database schema through the API to the client that consumes it.
- **Practical security habits.** Encrypted-at-rest records, short-lived codes, and least-privilege thinking are part of how I design things.
- **Range.** I move comfortably between database design, mobile UI, front-end craft, and 3D graphics, and I pick up new areas quickly.
- **Comfort near hardware.** I understand sampling rates, noisy sensor data, and the constraints devices put on the services that talk to them.
- **Maintainable by default.** Small dependency footprints, documented tooling, and sources that can be rebuilt by the next person.

---

## GitHub Activity

<p>
  <img height="165" alt="GitHub stats" src="https://github-readme-stats.vercel.app/api?username=TlNT0&show_icons=true&hide_border=true&theme=default" />
  <img height="165" alt="Top languages" src="https://github-readme-stats.vercel.app/api/top-langs/?username=TlNT0&layout=compact&hide_border=true" />
</p>

---

## Contact

Email: [rodrigo.rio.tinto@email.com](mailto:rodrigo.rio.tinto@email.com)
GitHub: [@TlNT0](https://github.com/TlNT0)

<div align="center">

# ⚡ Video Sniffer Pro (v1.0)
*A high-performance, autonomous media interceptor and HLS stream downloader built inside Chrome.*

</div>

## 🚀 Key Features

* **Multi-Threaded HLS/M3U8 Engine:** A complete, custom-built Transport Stream chunk compiler. It dynamically parses `.m3u8` master playlists, geometrically calculates the absolute highest resolution bandwidth, fetches individual `.ts` segments concurrently, and flawlessly merges them into an `.mp4` container directly on your machine.
* **Offscreen Background Processing:** Video generation is completely insulated from fragile UI menus. Heavy chunk merging and BLOB transfers execute securely within a detached, persistent background worker. You can safely close the extension interface while downloads effortlessly process in the background.
* **Dynamic Neon Real-Time UI:** Visually pleasing, neon-cyan visual progress overlays injected directly into the extension's interactive video cards, supplying accurate, real-time download completion percentages.
* **YouTube InnerTube Extraction:** Intelligently bypasses modern streaming firewalls and rigid `403 Forbidden` restrictions by masking as a `TVHTML5` client, pulling secure stream manifests directly from inner APIs.

---

## 🛠️ Installation Instructions

Since this is an unpacked extension, you can easily load it into any Chromium browser:
1. Download or clone this repository to a local folder.
2. Navigate to `chrome://extensions/` in your browser.
3. Toggle on **Developer mode** in the top right corner.
4. Click **Load unpacked** and select the directory containing this folder.

## ⚙️ Architecture & Tech Stack
- **Google Manifest V3:** Fully compliant with Chrome's modern strict security policies.
- **Service Workers:** Powers the core networking interception engine.
- **Offscreen Documents API:** Replaces old DOM architectures with state-of-the-art background compiling.
- **Vanilla JavaScript:** 0 Megabytes of third-party baggage. Zero libraries required.

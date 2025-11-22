 # Libre Hardware Monitor Web Panel

  A lightweight mobile-first dashboard for Libre Hardware Monitor data. 
  View CPU, GPU, VRAM, RAM, storage, and network telemetry from any device.

<img width="1460" height="1169" alt="image" src="https://github.com/user-attachments/assets/2ebd9b31-9536-4bf8-b1b4-33fd710d3996" />
<img width="1050" height="471" alt="image" src="https://github.com/user-attachments/assets/32f887f9-5ab8-495c-8f11-82569367a879" />
<img width="486" height="1082" alt="image" src="https://github.com/user-attachments/assets/38342a0c-b183-453e-b5ce-ae38febbecbe" />

  ## Features
  - Cockpit UI optimized for phones and tablets, with theme switching and collapsible detail sections.
  - Realtime polling of any Libre Hardware Monitor endpoint; configurable refresh interval and data URL.
  - Highlighted CPU/GPU temp & power gauges, VRAM usage, memory bar, NVMe read/write, and NIC selector for upload/download/utilization.
  - Minimal Node server (`server.js`) that serves `/public` and proxies `/data.json`; can be replaced by Nginx or any static host.

  ## Usage
  1. `PORT=8090 node server.js` (or just `node server.js` for the default 8085).
  2. Open `http://<host>:<port>/` on your phone, set the Endpoint to your actual `http://<device>:<port>/data.json`, and enjoy the cockpit.

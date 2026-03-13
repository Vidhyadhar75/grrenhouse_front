# 🌿 GreenHouse Control Center

A React dashboard for live greenhouse sensor monitoring.

## Folder Structure

```
src/
├── App.jsx                        # Root — layout, routing, global styles
│
├── hooks/
│   └── useLive.js                 # Sensor simulation hook (base, range, dec, ms)
│
├── components/
│   ├── Sidebar.jsx                # Left nav with logo, nav buttons, live badge
│   ├── NatureScene.jsx            # SVG hero scene (sky, greenhouse, trees...)
│   ├── PageShell.jsx              # Shared page header wrapper
│   ├── SensorCard.jsx             # Gradient card with value + sparkline
│   ├── GaugeCard.jsx              # Gradient card with semicircle gauge
│   ├── Gauge.jsx                  # Semicircle gauge with needle (SVG)
│   ├── Spark.jsx                  # Rolling sparkline chart (SVG)
│   └── MotorCard.jsx              # Clickable toggle card for motors
│
└── pages/
    ├── DashboardPage.jsx          # Overview: nature scene, 3 gauges, 3 sensor cards
    ├── AirQualityPage.jsx         # CO2, Temp, Humidity, Pressure, Gas
    ├── NPKPage.jsx                # Moisture, Temp, pH, EC, N, P, K
    ├── SoilPage.jsx               # Soil Moisture card + gauge
    ├── PowerPage.jsx              # Voltage, Current, Power
    ├── GHStatusPage.jsx           # Operational status display
    └── MotorsPage.jsx             # Motor 1 & Motor 2 toggles
```

## Getting Started

```bash
# Create a new Vite + React project and copy src/ into it
npm create vite@latest greenhouse-app -- --template react
cd greenhouse-app
# Replace the src/ folder with this one
npm install
npm run dev
```

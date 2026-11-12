# TerraSage

**Cooling intelligence for buildings, cities and homes.**

TerraSage is an urban cooling venture that combines an AI heat-risk platform with a layered cooling surface (PCM layer, reflective layer and radiative coating) for roofs, pavements, shade structures and walls. Built sensors measure the result, and the platform shows the savings in rupees.

This repository holds the **interactive prototype** made for the Wadhwani Foundation Venture Viability Analysis at VIT-AP University.

**Live demo:** https://aara-codex.github.io/TerraSage/

> **Important:** this is a prototype with simulated data. See "What is real, assumed and simulated" below.

## What the prototype shows

- **Overview:** the problem, the product and the market numbers.
- **Product in 3D:** the four layers, which you can pull apart, plus a simulated sensor scan.
- **Live install demo:** how TerraSage is installed on a roof, pavement, wall or shade structure.
- **City selection:** Vijayawada and Amaravati, Hyderabad, Chennai, Bengaluru, Mumbai and Ahmedabad, each with its own climate and tariff.
- **Explore:** a 3D heat-risk map and a real OpenStreetMap map of places in the chosen city. Customer segments are government and municipalities, commercial buildings, and local homes and shops.
- **Booking:** name, email and a validated 10-digit Indian mobile number.
- **Project:** the per-customer journey: sensor scan, findings, budget plan, install progress with dates, and month-one results.
- **Help desk:** complaints with a ticket tracker, a work and plan tracker, and feedback.

## What is real, assumed and simulated

**Real inputs (sourced):**

| Input | Source |
|---|---|
| Commercial tariff ₹9.95 per unit, cut from ₹12.25 (FY 2026–27, Andhra Pradesh) | APERC tariff order press note, aperc.gov.in |
| India peak electricity demand 148 GW (2014) to 250 GW (2024) | IEA, Electricity 2025 |
| Cooling demand about 8 times by 2037–38 compared with 2017–18 | India Cooling Action Plan (MoEFCC) |
| 2°C average indoor drop, 2017 Hyderabad pilot (25 homes, white reflective membrane) | NRDC, ASCI and IIIT-H |
| Cool roof coatings about ₹20 to 50 per sq ft applied | Vendor listings |
| Positions of the places on the map | OpenStreetMap |

**Our assumptions (to be confirmed at survey or pilot):** PCM and radiative layer prices, home and municipal tariffs, tariffs for cities other than Andhra Pradesh, 5% less cooling energy per °C of cooling, roof share of the cooling load, repair at ₹6 per sq ft, and sensors and gateway at ₹15,000.

**Simulated in the demo:** the buildings and their heat-risk scores, all sensor readings and month-one results, install progress, tickets, bookings and project numbers. Nothing is sent or stored: there is no backend, SMS or email.

The 2°C Hyderabad result supports the reflective layer only. The PCM and radiative layers need our own pilot.

## How it becomes real

1. Run a pilot on a few real roofs with surface and indoor sensors (ESP32).
2. Replace the assumptions above with measured readings.
3. Load real building footprints from OpenStreetMap and satellite temperature data in place of the modelled buildings.

## Tech

- Single-file web app (`index.html`) in plain HTML, CSS and JavaScript
- [Three.js](https://threejs.org/) for the 3D views
- [Leaflet](https://leafletjs.com/) and OpenStreetMap for the city map
- Hosted on GitHub Pages

## Run it locally

Download `index.html` and open it in a browser. It needs an internet connection for the 3D library, the map tiles and the fonts.

## Team

VIT-AP University, venture team of three: Anjum Aara (tech lead), A.S.V. Eshitha Sri and Shiva Varun.

## Credits

Map data © OpenStreetMap contributors.

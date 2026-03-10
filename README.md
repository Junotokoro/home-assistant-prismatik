<p align="center">
  <img src="https://raw.githubusercontent.com/zomfg/Lightpack/749b592dd033cc96240a75f16d85f170640fab50/Software/res/icons/Prismatik.png" width="80" />
  &nbsp;
  &nbsp;
  &nbsp;
  <img src="https://raw.githubusercontent.com/home-assistant/assets/1e19f0dca208f0876b274c68345fcf989de7377a/logo/logo-pretty.svg" width="80" />
</p>

<p align="center">
  <img src="https://github.com/Junotokoro/home-assistant-prismatik/actions/workflows/main.yml/badge.svg" />
  <a href="https://github.com/custom-components/hacs"><img src="https://img.shields.io/badge/HACS-Custom-orange.svg" /></a>
</p>

# Home Assistant Prismatik Integration

Integration for [Prismatik](https://github.com/psieg/Lightpack) backlight control  in Home Assistant.


## Installation

### HACS (Recommended)
1. Click the button below to add this custom repository to HACS\
[![Open your Home Assistant instance and open a repository inside the Home Assistant Community Store.](https://my.home-assistant.io/badges/hacs_repository.svg)](https://my.home-assistant.io/redirect/hacs_repository/?category=integration&repository=home-assistant-prismatik&owner=Junotokoro)
2. Install "Prismatik" from HACS
3. Restart Home Assistant
4. Add the integration through the UI or yaml


## Settings

### **Prismatik app**

> [!IMPORTANT]
> Before using, make sure that the `"Listen only on local interface (127.0.0.1)"` checkbox is unchecked in the Prismatik settings..


### **HA config**

you can configure the integration through UI
or with YAML
```yaml
light:
  - platform: prismatik
    host: 192.168.42.42

    # optional
    port: 3636

    # optional
    name: "Prismatik"

    # optional
    api_key: '{API_KEY}'

    # optional: profile name to use so other profiles don't get altered
    profile_name: hass
```

Tested on HA 2026.3 and Prismatik [5.11.2.31](https://github.com/psieg/Lightpack/releases/tag/5.11.2.31)

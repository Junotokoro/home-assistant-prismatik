<p align="center">
  <img src="https://raw.githubusercontent.com/zomfg/Lightpack/749b592dd033cc96240a75f16d85f170640fab50/Software/res/icons/Prismatik.png" width="80" />
  &nbsp;
  &nbsp;
  &nbsp;
  <img src="https://raw.githubusercontent.com/home-assistant/assets/1e19f0dca208f0876b274c68345fcf989de7377a/logo/logo-pretty.svg" width="80" />
</p>

<p align="center">
  <img src="https://github.com/zomfg/home-assistant-prismatik/workflows/Latest%20HA/badge.svg?branch=master&event=schedule" />
  <a href="https://github.com/custom-components/hacs"><img src="https://img.shields.io/badge/HACS-Custom-orange.svg" /></a>
</p>

**Prismatik**

uncheck `Listen only on local interface`

**HA server**

Add the repo to HACS and install from there

or manually download to `/hass/config/custom_components` and rename `home-assistant-prismatik` to `prismatik`


**HA config**

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

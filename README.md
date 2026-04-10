# Google Dark Theme

A Home Assistant theme inspired on Google app dark mode.

> **Fork notice:** this is a maintained fork of [JuanMTech/google_dark_theme](https://github.com/JuanMTech/google_dark_theme), which has been inactive since 2023.
<br />
<br />

### Home Assistant 2026.4+ compatibility

The Home Assistant 2026.4 frontend migrated `ha-textfield` to `ha-input` and dropped the old `mdc-text-field-fill-color` / `mdc-select-fill-color` / `input-fill-color` theme variables. That caused dropdowns and text fields (Language, Theme, Dashboard, etc.) to render with a bright white background on this dark theme.

This fork adds the new semantic form variables introduced in 2026.4 so text fields render correctly again:

- `ha-color-form-background`
- `ha-color-form-background-hover`
- `ha-color-form-background-disabled`

See the [frontend 2026.4 component update](https://developers.home-assistant.io/blog/2026/03/25/frontend-component-updates-2026.4/) for background.
<br />
<br />

[![hacs_badge](https://img.shields.io/badge/HACS-Default-orange.svg?style=for-the-badge)](https://github.com/custom-components/hacs)


[![Subscribe to YouTube channel][youtube-sub-shield]][youtubesubscribe]

[![Become a Patron][become-a-patron-shield]][becomeapatron]

[![Buy me a coffee][buymeacoffee-shield]][buymeacoffee]
<br />
<br />

### Screenshots

![Google Dark Mode 1](https://raw.githubusercontent.com/JuanMTech/google_dark_theme/master/images/Google%20Dark%20Mode%201.jpg)<br />
<br />

### Preparation
1. Make sure that under the **configuration.yaml** file you have the following:

```
frontend:
  themes: !include_dir_merge_named themes
```

2. Under the Home Assistant **Config** folder, create a new folder named **themes**
3. **Restart** Home assistant to apply the changes. 

### HACS installation

This fork is not in the HACS default index, so it has to be added as a custom repository:

1. Open **HACS** in Home Assistant.
2. Click the three-dot menu (top right) → **Custom repositories**.
3. Repository: `https://github.com/notownblues/google_dark_theme`
4. Type: **Theme**, then click **Add**.
5. Search for **Google Dark Theme** in HACS and open it.
6. Press **Download**.
7. Restart Home Assistant.

### Manual installation
1. In the Home assistant **themes** folder, create a file named `google_dark_theme.yaml`
2. In this GitHub repo, go into the **themes** folder, open the `google_dark_theme.yaml` file and copy the content
3. Paste the content in the `google_dark_theme.yaml` file created under your Home Assistant themes folder

### Enable theme
1. Open your Home Assistant **Profile**
2. Under, **Themes**, select the new Google Dark Theme


### Custom Header settings
When using the [Custom Header](https://github.com/maykar/custom-header) plugin, add the following to make sure that the header matches the theme.

<br />
<br />
<br />

# Other available themes
- [**iOS Theme**](https://github.com/JuanMTech/ios-theme) - Based on the system-wide light and dark mode UI
- [**Google Theme**](https://github.com/JuanMTech/google-theme) - Based on the Android light and dark interface
- [**AMOLED Blue**](https://github.com/JuanMTech/amoled_blue) - A true black Home Assistant theme for devices with AMOLED displays



[buymeacoffee-shield]: https://i.imgur.com/Hzn2rM8.png
[buymeacoffee]: https://www.buymeacoffee.com/JuanMTech
[become-a-patron-shield]: https://i.imgur.com/U9BjCfc.png
[becomeapatron]: https://www.patreon.com/JuanMTech
[youtube-sub-shield]: https://i.imgur.com/6TAqHgi.png
[youtubesubscribe]: https://www.youtube.com/c/JuanMTech?sub_confirmation=1

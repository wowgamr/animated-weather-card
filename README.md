# Animated Weather Card
Animated icons for default Home Assistant [weather card](https://www.home-assistant.io/lovelace/weather-forecast/)

[![hacs_badge](https://img.shields.io/badge/HACS-Default-orange.svg)](https://github.com/hacs/integration)

### Screenshots
![](https://clients.wowgamr.ru/hacs/weather1.gif)
![](https://clients.wowgamr.ru/hacs/weather2.gif)

### Preparation
1. Make sure that under the **configuration.yaml** file you have the following:
<pre>
frontend:
  themes: !include_dir_merge_named themes
</pre>
2. Under the Home Assistant **Config** folder, create a new folder named **themes**
3. **Restart** Home Assistant to apply the changes

### HACS installation
1. Go into the Community Store (HACS)
2. Search for **Animated Weather Card**
3. Press Install
4. Move `themes/animated-weather-card/icons/*` to `www/community/animated-weather-card/icons/*` via ssh/samba/etc
5. Restart Home Assistant

### Manual installation
1. In the Home Assistant **themes** folder, create a folder named `animated-weather-card`
2. [Download](https://github.com/wowgamr/animated-weather-card/releases) latest release source code
3. Unarchive .yaml file from **themes** folder into `animated-weather-card`
4. In the Home Assistant **www/community** folder, create a folder named `animated-weather-card`
5. Unarchive icons folder from **themes** folder into `www/community/animated-weather-card`
6. Check paths. They must be `/config/themes/animated-weather-card/animated-weather-card.yaml` and `/www/community/animated-weather-card/icons/clear-night.svg`

### Enable theme
1. Open editing your weather card
2. Select **Animated Weather Card** as **Theme**

### Manual installation (for existing theme)
1. [Download](https://github.com/wowgamr/animated-weather-card/releases) latest release source code
2. Unarchive **icons** folder into your theme folder, located in `/www/community/`
3. Copy variables from `animated-weather-card.yaml`
4. Check icon paths. `/hacsfiles/` is virtual path of `/www/community/`. For icon placed in `/www/community/you_theme_folder_name/icons/clear-night.svg` variable's path is `/hacsfiles/you_theme_folder_name/icons/clear-night.svg`

### Credits
amCharts icons - [https://www.amcharts.com/free-animated-svg-weather-icons](https://www.amcharts.com/free-animated-svg-weather-icons/)

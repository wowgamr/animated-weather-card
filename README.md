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
2. Press menu icon and select **Custom repositories**
3. Add new repository
<pre>
url: https://github.com/wowgamr/animated-weather-card
category: Theme
</pre>
4. Open the theme in **Frontend** tab
5. Press Install
6. Restart Home Assistant

### Manual installation
1. In the Home Assistant **themes** folder, create a folder named `animated-weather-card`
2. [Download](https://github.com/wowgamr/animated-weather-card/releases) latest release source code
3. Unarchive files from **themes** folder into `animated-weather-card`
4. Check paths. They must be `/config/themes/animated-weather-card/animated-weather-card.yaml` and `/config/themes/animated-weather-card/icons/clear-night.svg`

### Enable theme
1. Open your Home Assistant **Profile**
2. Under **Themes** select **Animated Weather Card**

### Manual installation (for existing theme)
1. [Download](https://github.com/wowgamr/animated-weather-card/releases) latest release source code
2. Unarchive **icons** folder into your theme folder
3. Copy variables from `animated-weather-card.yaml`
4. Check icon paths. `/hacsfiles/themes/` is virtual path of `/config/themes/`. So for icon placed in `/config/themes/you_theme_folder_name/icons/clear-night.svg` variable's path is `/hacsfiles/themes/animated-weather-card/icons/clear-night.svg`

### Credits
amCharts icons - [https://www.amcharts.com/free-animated-svg-weather-icons](https://www.amcharts.com/free-animated-svg-weather-icons/)

# Darkerr [![Version](https://img.shields.io/badge/version-2.6-ED1C24.svg?longCache=true&style=flat-square)](#) [![userstyles.org installations](https://img.shields.io/badge/dynamic/json.svg?label=userstyles.org%20installations&url=https%3A%2F%2Fwidget.userstyles.org%2Fstyles%2F142759%2Fdarkerr-a-darker-theme-for-sonarr-radarr.json&query=total_installs&colorB=e51ced&longCache=true&style=flat-square)](https://userstyles.org/styles/142759/darkerr-a-darker-theme-for-sonarr-radarr) [![GitHub stars](https://img.shields.io/github/stars/iFelix18/Darkerr.svg?longCache=true&style=flat-square)](https://github.com/iFelix18/Darkerr/stargazers) [![GitHub issues](https://img.shields.io/github/issues/iFelix18/Darkerr.svg?longCache=true&style=flat-square)](https://github.com/iFelix18/Darkerr/issues) [![GitHub license](https://img.shields.io/github/license/iFelix18/Darkerr.svg?longCache=true&style=flat-square)](https://creativecommons.org/licenses/by-sa/4.0/)
**_A darker theme for Sonarr &amp; Radarr_**
<p align="center">
 <a href="https://github.com/iFelix18/Darkerr/blob/master/README.md#screenshot">
  <img src="https://i.imgur.com/sz99ZPq.jpg" title="Click to see more screenshots" alt="Darkerr"/>
 </a>
</p>

# Menu
* [Installation](https://github.com/iFelix18/Darkerr/blob/master/README.md#installation)
  * [Server-side installation (with nginx)](https://github.com/iFelix18/Darkerr/blob/master/README.md#server-side-installation)
* [Optional additional themes:](https://github.com/iFelix18/Darkerr/blob/master/README.md#optional-additional-themes)
  * [Hide the searchbar](https://github.com/iFelix18/Darkerr/blob/master/README.md#hide-the-searchbar)
  * [Animate the logo](https://github.com/iFelix18/Darkerr/blob/master/README.md#animate-the-logo)
* [Screenshot](https://github.com/iFelix18/Darkerr/blob/master/README.md#screenshot)
# Installation
* Download one of these add-ons for your browser
  * Stylus (recommended): [Chrome](https://chrome.google.com/webstore/detail/clngdbkpkpeebahjckkjfobafhncgmne), [Firefox](https://addons.mozilla.org/firefox/addon/styl-us/), or [Opera](https://github.com/schomery/stylish-chrome/).
  * Osprey: [Chrome](https://chrome.google.com/webstore/detail/osprey/ekjapccimkannnfgcnnoajhfdglobgak).
  * Stylish: [Chrome](https://chrome.google.com/webstore/detail/stylish-custom-themes-for/fjnbnpbmkenffdnngjfgmeleoegfcffe), [Firefox](https://addons.mozilla.org/en-US/firefox/addon/stylish/), and [Opera](https://addons.opera.com/en-gb/extensions/details/stylish/).
* Go [userstyles.org](https://userstyles.org/styles/142759/darkerr-a-darker-theme-for-sonarr-radarr), and click on "Install Style" button.
* Done! From now on it will automatically update.

You do not use the default ports (8989 for Sonarr and 7878 for Radarr)?
If so, just change the string in the settings, from:
```
((http(s?))://)?[-A-Za-z0-9+&@#/%?=~_|!:,.;]+(8989|7878|sonarr|radarr)+(.*)
```
to:
```
((http(s?))://)?[-A-Za-z0-9+&@#/%?=~_|!:,.;]+(your sonarr port|your radarr port|sonarr|radarr)+(.*)
```
(Note: for each update, this change must be done again)

* # Server-side installation (with nginx)
  * Add these lines to your Sonarr/Radarr location blocks in nginx.conf:
    ```
    proxy_set_header Accept-Encoding "";
    sub_filter
     '</head>'
     '<link rel="stylesheet" type="text/css" href="//rawgit.com/iFelix18/Darkerr/master/darkerr.css">
     </head>';
    sub_filter_once on;
    ```
    or with optional additional themes:
    ```
    proxy_set_header Accept-Encoding "";
    sub_filter
     '</head>'
     '<link rel="stylesheet" type="text/css" href="//rawgit.com/iFelix18/Darkerr/master/darkerr.css">
      <link rel="stylesheet" type="text/css" href="//rawgit.com/iFelix18/Darkerr/master/logo_animation.css">
      <link rel="stylesheet" type="text/css" href="//rawgit.com/iFelix18/Darkerr/master/hidden_searchbar.css">
     </head>';
    sub_filter_once on;
    ```
  * Restart nginx. Done!
  
# Optional additional themes
<details>
 
* # Hide the searchbar
  <p align="center">
    <img src="http://i.imgur.com/6sdDzxq.gif" alt="searchbar"/>
  </p>
  <p>Download <a href="https://userstyles.org/styles/142942/darkerr-searchbar-theme-for-sonarr-radarr">here</a>.</p>

* # Animate the logo
  <p align="center">
    <img src="http://i.imgur.com/2Ie6BFm.gif" alt="logo"/>
  </p>
  <p>Download <a href="https://userstyles.org/styles/142943/darkerr-logo-theme-for-sonarr-radarr">here</a>.</p>
</details>

# Screenshot
<details>
 <p align="center">
  Detailed view:
  <img src="https://i.imgur.com/aHxTA5c.jpg" alt="detailed view"/>
 </p>
 <p align="center">
  Overview list:
  <img src="https://i.imgur.com/DHDo6uS.jpg" alt="overview list"/>
 </p>
</details>

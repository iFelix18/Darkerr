# Darkerr v2 [![Version][version]][1] [![GitHub stars][stars]][2] [![GitHub issues][issues]][3] [![GitHub license][license]][4]
**_A darker theme for [Sonarr] v2 &amp; [Radarr] v0_**

**UNMAINTAINED VERSION!!!**</br>
Please, update to Sonarr v3 and to Radarr v1 and use [Darkerr v3]

[![Preview][preview]][Screenshots]

# Menu
* [Installation]
  * [Server-side installation] (for, eg,  _"http://<span></span>localhost/sonarr"_)
  * [Browser-side installation] (for, eg,  _"http://<span></span>localhost/8989"_)
* [Optional additional themes]
  * [Hide the searchbar]
  * [Animate the logo]
* [Screenshots]

## Installation
* ### Server-side installation
  * Add these lines to your Sonarr/Radarr location blocks in nginx.conf:
    ```nginx		
    proxy_set_header Accept-Encoding "";
    sub_filter
      '</head>'
      '<link rel="stylesheet" type="text/css" href="//raw.githack.com/iFelix18/Darkerr/master/v2/darkerr.css">
       </head>';
    sub_filter_once on;
    ```
  * Restart nginx.
  * Done! From now on it will automatically update.

* ### Browser-side installation
  * Download this add-on for your browser
    * Stylus: [Firefox][5], [Chrome][6],  or [Opera][7].
  * Go [userstyles.org][1], and click on "Install Style" button.
  * Done! From now on it will automatically update.
  
## Optional additional themes
<details><summary>Show</summary>

* ### Hide the searchbar
  <p align="center">
    <img src="https://i.imgur.com/6sdDzxq.gif" alt="searchbar"/>
  </p>

  Install it on server-side, by adding these line to your Sonarr/Radarr location blocks in nginx.conf:
    ```diff
    proxy_set_header Accept-Encoding "";
      sub_filter
        '</head>'
        '<link rel="stylesheet" type="text/css" href="//raw.githack.com/iFelix18/Darkerr/master/v2/darkerr.css">
    +    <link rel="stylesheet" type="text/css" href="//raw.githack.com/iFelix18/Darkerr/master/v2/logo_animation.css">
         </head>';
      sub_filter_once on;
    ```

    Or browser-side with Stylus by going [here][searchbar].

* ### Animate the logo
  <p align="center">
    <img src="https://i.imgur.com/2Ie6BFm.gif" alt="logo"/>
  </p>

  Install it on server-side, by adding these line to your Sonarr/Radarr location blocks in nginx.conf:
    ```diff
    proxy_set_header Accept-Encoding "";
      sub_filter
        '</head>'
        '<link rel="stylesheet" type="text/css" href="//raw.githack.com/iFelix18/Darkerr/master/v2/darkerr.css">
    +    <link rel="stylesheet" type="text/css" href="//raw.githack.com/iFelix18/Darkerr/master/v2/hidden_searchbar.css">
         </head>';
      sub_filter_once on;
    ```
    Or browser-side with Stylus by going [here][logo].
</details>

## Screenshots
<details><summary>Show</summary>

  ![Detailed view][detailed view]
  ![Overview list][overview list]
</details>

[version]: https://flat.badgen.net/badge/version/2.6/ED1C24
[1]: https://userstyles.org/styles/142759/darkerr-a-darker-theme-for-sonarr-radarr
[stars]: https://flat.badgen.net/github/stars/iFelix18/Darkerr
[2]: https://github.com/iFelix18/Darkerr/stargazers
[issues]: https://flat.badgen.net/github/open-issues/iFelix18/Darkerr
[3]: https://github.com/iFelix18/Darkerr/issues
[license]: https://flat.badgen.net/github/license/iFelix18/Darkerr
[4]: https://creativecommons.org/licenses/by-sa/4.0/

[Sonarr]: https://github.com/Sonarr/Sonarr
[Radarr]: https://github.com/Radarr/Radarr

[Darkerr v3]: /README.md

[preview]: https://i.imgur.com/sz99ZPq.jpg "Click to see more screenshots"

[Installation]: README.md#installation
[Server-side installation]: README.md#server-side-installation
[Browser-side installation]: README.md#browser-side-installation
[Optional additional themes]: README.md#optional-additional-themes
[Hide the searchbar]: README.md#hide-the-searchbar
[Animate the logo]: README.md#animate-the-logo
[Screenshots]: README.md#screenshots

[5]: https://addons.mozilla.org/firefox/addon/styl-us/
[6]: https://chrome.google.com/webstore/detail/clngdbkpkpeebahjckkjfobafhncgmne
[7]: https://addons.opera.com/extensions/details/stylus/

[searchbar]: https://userstyles.org/styles/142942/darkerr-searchbar-theme-for-sonarr-radarr
[logo]: https://userstyles.org/styles/142943/darkerr-logo-theme-for-sonarr-radarr

[detailed view]: https://i.imgur.com/aHxTA5c.jpg
[overview list]: https://i.imgur.com/DHDo6uS.jpg

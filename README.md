# Darkerr [![Version][version]][1] [![Install directly with Stylus][stylus]][2] [![GitHub stars][stars]][3] [![GitHub issues][issues]][4] [![GitHub license][license]][5]
**_A darker theme for [Sonarr], [Radarr] &amp; [Lidarr]_**

## Menu
* [Installation]
    * [Server-side installation (with nginx)]
    * [Browser-side installation (with Stylus)]
* [Screenshots]

## Installation
* ### Server-side installation
    * Add these lines to your Sonarr/Radarr/Lidarr location blocks in nginx.conf:
    ```nginx		
    proxy_set_header Accept-Encoding "";
    sub_filter
        '</head>'
        '<link rel="stylesheet" type="text/css" href="https://rawgit.com/iFelix18/Darkerr/develop/darkerr.css">
        </head>';
    sub_filter_once on;
    ```
  * Restart nginx.
  * Done! From now on it will automatically update.

* ### Browser-side installation
    * Download this add-on for your browser
        * Stylus: [Firefox][5], [Chrome][6],  or [Opera][7].
    * Click [here][2] to install directly with Stylus.
    * Done! From now on it will automatically update.

## Screenshots
<details><summary>Show</summary>
</details>

[version]: https://img.shields.io/badge/version-3.0.0--beta2-ED1C24.svg?longCache=true&style=flat-square
[1]: #
[stylus]: https://img.shields.io/badge/install%20directly%20with-Stylus-00adad.svg?longCache=true&style=flat-square "Click here!"
[2]: https://rawgit.com/iFelix18/Darkerr/develop/darkerr.user.css
[stars]: https://img.shields.io/github/stars/iFelix18/Darkerr.svg?longCache=true&style=flat-square
[3]: https://github.com/iFelix18/Darkerr/stargazers
[issues]: https://img.shields.io/github/issues/iFelix18/Darkerr.svg?longCache=true&style=flat-square
[4]: https://github.com/iFelix18/Darkerr/issues
[license]: https://img.shields.io/github/license/iFelix18/Darkerr.svg?longCache=true&style=flat-square
[5]: https://creativecommons.org/licenses/by-sa/4.0/

[Sonarr]: https://github.com/Sonarr/Sonarr
[Radarr]: https://github.com/Radarr/Radarr
[Lidarr]: https://github.com/lidarr/Lidarr

[Installation]: README.md#installation
[Server-side installation (with nginx)]: README.md#server-side-installation
[Browser-side installation (with Stylus)]: README.md#browser-side-installation
[Screenshots]: README.md#screenshots

[5]: https://addons.mozilla.org/firefox/addon/styl-us/
[6]: https://chrome.google.com/webstore/detail/clngdbkpkpeebahjckkjfobafhncgmne
[7]: https://addons.opera.com/extensions/details/stylus/

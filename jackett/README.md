# Darkerr for Jackett [![Version][version]][1] [![Install directly with Stylus][stylus]][2] [![GitHub stars][stars]][3] [![GitHub issues][issues]][4] [![GitHub license][license]][5]
**_A darker theme for [Jackett]_**

## Menu
* [Installation]
    * [Server-side installation] (for, eg,  _"http://<span></span>localhost/jackett"_)
    * [Browser-side installation] (for, eg,  _"http://<span></span>localhost/9117"_)
* [Screenshots]

## Installation
* ### Server-side installation
    * Add these lines to your Jackett location blocks in nginx.conf:
    ```nginx		
    proxy_set_header Accept-Encoding "";
    sub_filter
        '</head>'
        '<link rel="stylesheet" type="text/css" href="https://raw.githubusercontent.com/iFelix18/Darkerr/develop/jackett/darkerr.css">
        </head>';
    sub_filter_once on;
    ```
  * Restart nginx.
  * Done! From now on it will automatically update.

* ### Browser-side installation
    * Download this add-on for your browser
        * Stylus: [Firefox][6], [Chrome][7],  or [Opera][8].
    * Click [here][2] to install directly with Stylus.
    * Done! From now on it will automatically update.</br></br>

## Screenshots
<details><summary>Show</summary>
</details>

[version]: https://img.shields.io/badge/version-1.0.0--beta3-ED1C24.svg?longCache=true&style=flat-square
[1]: #
[stylus]: https://img.shields.io/badge/install%20directly%20with-Stylus-00adad.svg?longCache=true&style=flat-square "Click here!"
[2]: https://raw.githubusercontent.com/iFelix18/Darkerr/develop/jackett/darkerr.user.css
[stars]: https://img.shields.io/github/stars/iFelix18/Darkerr.svg?longCache=true&style=flat-square
[3]: https://github.com/iFelix18/Darkerr/stargazers
[issues]: https://img.shields.io/github/issues/iFelix18/Darkerr.svg?longCache=true&style=flat-square
[4]: https://github.com/iFelix18/Darkerr/issues
[license]: https://img.shields.io/github/license/iFelix18/Darkerr.svg?longCache=true&style=flat-square
[5]: https://creativecommons.org/licenses/by-sa/4.0/

[Jackett]: https://github.com/Jackett/Jackett

[Installation]: README.md#installation
[Server-side installation]: README.md#server-side-installation
[Browser-side installation]: README.md#browser-side-installation
[Screenshots]: README.md#screenshots

[6]: https://addons.mozilla.org/firefox/addon/styl-us/
[7]: https://chrome.google.com/webstore/detail/clngdbkpkpeebahjckkjfobafhncgmne
[8]: https://addons.opera.com/extensions/details/stylus/

# Darkerr [![Version][version]][1] [![Install directly with Stylus][stylus]][2] [![GitHub stars][stars]][3] [![GitHub issues][issues]][4] [![GitHub license][license]][5]
**_A darker theme for [Sonarr], [Radarr] &amp; [Lidarr]_**

**NOTICES:**
- Darkerr v3 works only on Sonarr v3 and Lidarr (soon also Radarr v1)
- If you use an old versions (Sonarr v2 and Radarr v0), take a look at [Darkerr v2]

## Menu
* [Installation]
    * [Server-side installation] (for, eg,  _"http://<span></span>localhost/sonarr"_)
    * [Browser-side installation] (for, eg,  _"http://<span></span>localhost/8989"_)
* [Screenshots]

## Installation
* ### Server-side installation
    * Add these lines to your Sonarr/Radarr/Lidarr location blocks in nginx.conf:
        ```nginx
        proxy_set_header Accept-Encoding "";
        sub_filter
            '</head>'
            '<link rel="stylesheet" type="text/css" href="//raw.githack.com/iFelix18/Darkerr/develop/darkerr.css">
             </head>';
        sub_filter_once on;
        ```
  * Restart nginx.
  * Done! From now on it will automatically update.

* ### Browser-side installation
    * Download this add-on for your browser
        * Stylus: [Firefox][6], [Chrome][7],  or [Opera][8].
    * Click [here][2] to install directly with Stylus.
    * Done! From now on it will automatically update.

    You do not use the default ports (8989 for Sonarr, 7878 for Radarr and 8686 for Lidarr)?
    <details><summary>Answer</summary>
    If so, just change this string via Stylus:

    ```diff
        [...]
        @updateURL      https://raw.githubusercontent.com/iFelix18/Darkerr/develop/darkerr.user.css
        @license        CC-BY-SA-4.0
        ==/UserStyle== */
    -   @-moz-document regexp("((http(s?)):\\/\\/)?[-A-Za-z0-9+&@#/%?=~_|!:,.;]+(8989|7878|8686)+(.*)") {
    +   @-moz-document regexp("((http(s?)):\\/\\/)?[-A-Za-z0-9+&@#/%?=~_|!:,.;]+(your custom Sonarr port|your custom Radarr port|your custom Lidarr port)+(.*)") {
        /* --- VERSION --- */
        @media (min-width: 768px) {
            .About-descriptionList-1_gea.DescriptionList-descriptionList-2MSh3 > span:nth-child(1) > .DescriptionListItemTitle-title-EA460:after {
        [...]
    ```
    (Note: for each update of Darkerr, this change must be done again)
    </details>

## Screenshots
<details><summary>Show</summary>
</details>

[version]: https://flat.badgen.net/badge/version/3.0.0-beta8/ED1C24
[1]: #
[stylus]: https://flat.badgen.net/badge/install%20directly%20with/Stylus/00ADAD "Click here!"
[2]: https://raw.githubusercontent.com/iFelix18/Darkerr/develop/darkerr.user.css
[stars]: https://flat.badgen.net/github/stars/iFelix18/Darkerr
[3]: https://github.com/iFelix18/Darkerr/stargazers
[issues]: https://flat.badgen.net/github/open-issues/iFelix18/Darkerr
[4]: https://github.com/iFelix18/Darkerr/issues
[license]: https://flat.badgen.net/github/license/iFelix18/Darkerr
[5]: https://creativecommons.org/licenses/by-sa/4.0/

[Sonarr]: https://github.com/Sonarr/Sonarr
[Radarr]: https://github.com/Radarr/Radarr
[Lidarr]: https://github.com/Lidarr/Lidarr

[Darkerr v2]: v2/README.md

[Installation]: README.md#installation
[Server-side installation]: README.md#server-side-installation
[Browser-side installation]: README.md#browser-side-installation
[Screenshots]: README.md#screenshots

[6]: https://addons.mozilla.org/firefox/addon/styl-us/
[7]: https://chrome.google.com/webstore/detail/clngdbkpkpeebahjckkjfobafhncgmne
[8]: https://addons.opera.com/extensions/details/stylus/

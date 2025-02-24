# docs.mjcb.ca #

This is the Git repository is for the **docs.mjcb.ca** website that is currently using the Hugo CMS platform and is deployed using the Netlify platform. This website hosts various documentation for the [mjcb.ca](https://mjcb.ca/) website, as well as other documentation from other sources.

This website was migrated from the **docs.mjcb.ca** domain in early 2025.

## Theme ##

This website uses the [Geekdoc](https://github.com/thegeeklab/hugo-geekdoc) theme.

## License ##

[![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]

This work is licensed under a [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License][cc-by-nc-sa].

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg

See the [LICENSE](https://github.com/mjcb-public/docs.mjcb.ca/blob/main/LICENSE) file for details.

## Netlify Status ##

[![Netlify Status](https://api.netlify.com/api/v1/badges/f124f940-914e-4c7f-a10e-fe471dcc11de/deploy-status)](https://app.netlify.com/sites/docsmjcbca/deploys)

## File and Folder Structure ##

```
.
├── /
│   ├── content/
│   ├── layouts/
│   │   └── partials/
│   │       └── gdpr-notice.html
│   ├── static/
│   │   ├── docs/
|   |   ├── gdpr-notice/
│   │   │   ├── gdpr-notice.css
│   │   │   └── gdpr-notice.js
|   |   ├── images/
|   |   └── robots.txt
│   └── themes/
|       └── hugo-geekdoc/
├── config.toml
├── LICENSE
├── netlify.toml
└── README.md
```

### Important Files ###

* **/config.toml** - Primary configuration file for Hugo. It is in TOML format.
* **/LICENSE** - License information for this website.
* **/netlify.toml** - Primary configuration file for Hugo deployment on the Netlify platform. It is in TOML format.
* **/README.md** - This README file.

### Important Folders ###

* **/content/** - Contains all posts.
* **/layouts/partials/** - Contains all partial templates which are added to the existing theme.
* **/static/** - Contains all content that is placed in the root of the website when rendered by Hugo.
* **/static/docs/** - Contains all linked documents for posts. Directories are named to match the post.
* **/static/gdpr-notice/** - Contains the necessary files for the GDPR notice for the website (if necessary).
* **/static/images/** - Contains all images.

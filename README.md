# Hexo Cheatsheets Theme
[![This project is using Percy.io for visual regression testing.](https://percy.io/static/images/percy-badge.svg)](https://percy.io/glaze/cheatsheets)
[![Netlify Status](https://api.netlify.com/api/v1/badges/5df0cfa1-c9c6-4898-a2cb-f99a2ac72585/deploy-status)](https://cheatsheetspreview.netlify.com/)
[![Commitizen friendly](https://img.shields.io/badge/commitizen-friendly-brightgreen.svg)](http://commitizen.github.io/cz-cli/)

A new **cheatsheets** theme for Hexo.
The design is from [devhints](http://devhints.io)

- [Preview](http://cheatsheets.inevitable.tech)
- [A post about it](https://www.inevitable.tech/posts/59f1905d/)

## Installation

### Install

```bash
$ git clone https://github.com/glazec/hexo-cheatsheets.git
```

### Enable

Modify `theme` setting in `_config.yml` to `hexo-cheatsheets`.

Disable default code highlight plugin in `_config.yml`.

```yml
highlight:
  enable: false
```

### Update

```bash
cd themes/hexo-cheatsheets
git pull
```

## Configuration

In `/themes/hexo-cheatsheets/_config.yml`: 

```yml
# The following are settings of the button in the upper-right corner.

github: "the link the github button point to"
githubToolTip: "Text displayed when hovering on the github button"
githubIcon: "URL for Github icon"
githubIconHover: "URL for Github icon on hover"

footer: false # set it true to enable footer

# The following are favicon settings.
# You can visit https://realfavicongenerator.net/ for more information and generate your favicon and apply it for your site.

favicon:
  favicon: "favicon URL"
  appleTouchIcon: "apple-touch-icon URL"
  icon32: "favicon 32x32 URL"
  icon16: "favicon 16x16 URL"
  manifest: "site.webmanifest URL"
  maskIcon: "safari-pinned-tab IRL"
  themeColor: "#F1F3F5" # theme color
```

When you enable `footer`, you can set ICP license and police license in `/config.yml`:

```yml
ICP_license: "京ICP备12345678号-1"
police_license: "京公网安备 12345678901234号"
```

## Writing

When using tht code block in the markdown, please write the language. Otherwise the highlight will not work.

The following example is correct.(Please **omit** the last dot, thant is a render issue)

```
```yml
favicon: "favicon url"
github: "the link the github button point to"
githubToolTip: "Text displayed when hovering on the github button"
```·


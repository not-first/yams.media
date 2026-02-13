yams.media
==========

This are the source files for https://yams.media.

## Dependencies

- Material for MkDocs (installed globally)

## Setup

### Install Material for MkDocs globally

``` sh
pip install mkdocs-material
```

### Clone and run

``` sh
git clone git@gitlab.com:rogs/yams.media.git
cd yams.media
```

### For local development

``` sh
mkdocs serve
```
And open http://127.0.0.1:8000 to see the site with live reload.

### For production build

``` sh
mkdocs build
```

Your files will be in the `./site` folder, ready to upload to a server.

**Note:** Automated deployment uses the existing build process via `.gitea/workflows/deploy.yml` and `build.sh`.

## Contributors

<a href="https://github.com/rogsme/yams/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=rogsme/yams" />
</a>
<a href="https://github.com/rogsme/yams.media/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=rogsme/yams.media" />
</a>

Made with [contrib.rocks](https://contrib.rocks).

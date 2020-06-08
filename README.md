# Heroku buildpack: Zip

This is a [Heroku buildpack](http://devcenter.heroku.com/articles/buildpack) for downloading and uncompressing zip files.

Files are downloaded with `wget` and uncompressed with `unzip`.

## Usage

Example usage:

```bash
$ echo http://some/zip/url.zip > zipfile.txt
$ heroku buildpacks:add http://github.com/nilox94/heroku-buildpack-zip.git
$ git add zipfile.txt
$ git commit -m "Add zip buildpack"
$ git push heroku master
```


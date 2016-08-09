# Heroku Buildpack: wkhtmltopdf

Downloads wkhtmlto* binaries, verifies, then copies bin/

## Tested against following

- wkhtmltopdf 0.12.3

## Usage

```
$ heroku buildpacks:set https://github.com/issueapp/heroku-buildpack-wkhtmltopdf

$ heroku config:set WKHTMLTOPDF_URL=http://download.gna.org/wkhtmltopdf/0.12/0.12.3/{wkhtmltox-0.12.3_linux-generic-amd64.tar.xz,SHA1SUMS}

$ git commit --allow-empty
$ git push heroku

$ heroku run bin/wkhtmltopdf -V

# profit!
```

## Reference

(Heroku Buildpacks)[https://devcenter.heroku.com/articles/buildpacks]

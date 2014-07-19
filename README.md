heroku-selectable-procfile
==========================

## Usage

It's very simple.  This buildpack just moves the Procfile located at `$PROCFILE_PATH` to ./Procfile.  Use with [heroku-buildpack-multi](https://github.com/ddollar/heroku-buildpack-multi) to customize which Procfile Heroku runs.

```
$ heroku config:add BUILDPACK_URL=https://github.com/ddollar/heroku-buildpack-multi.git
$ heroku config:add PROCFILE_PATH=deployment/heroku/Procfile.heroku

$ cat .buildpacks
https://github.com/cantino/heroku-selectable-procfile.git
https://github.com/heroku/heroku-buildpack-ruby.git
```

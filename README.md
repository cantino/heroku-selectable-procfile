heroku-selectable-procfile
==========================

## Usage

Add this buildpack to your Heroku app buildpacks :

    $ heroku buildpacks:add https://github.com/cantino/heroku-selectable-procfile

Specify your custom Procfile path in the environment variables :

    $ heroku config:add PROCFILE_PATH=Procfile.custom

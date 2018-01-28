Heroku buildpack: Bluemix CLI (bx)
=======================

This is a [Heroku buildpack](http://devcenter.heroku.com/articles/buildpacks) of [Bluemix CLI (bx)](https://console.bluemix.net/docs/cli/index.html).

Usage
-----

Example usage:

    [your app]
    $ heroku create --buildpack http://github.com/mallowlabs/heroku-buildpack-bluemix-cli.git
    $ heroku config:add BLUEMIX_API_KEY=<your token>
    $ heroku config:add BLUEMIX_API_ENDPOINT=https://api.ng.bluemix.net
    $ heroku config:add BLUEMIX_ORG=<your organization>
    $ heroku config:add BLUEMIX_SPACE=<your space>
    $ git push heroku master
    $ heroku run bx cf help


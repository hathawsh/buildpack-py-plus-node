This tiny Heroku buildpack runs a Python backend that depends on a
static webpack-compiled frontend.  I use it with the following .buildpacks
file:

    backend=https://github.com/heroku/heroku-buildpack-python.git
    backend=https://github.com/hathawsh/heroku-buildpack-buildout.git
    frontend=https://github.com/heroku/heroku-buildpack-nodejs.git
    https://github.com/hathawsh/buildpack-py-plus-node

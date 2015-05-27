# Buildpack for Jupyter and Conda
This buildpack combines [conda][] with [jupyter][] to allow you to easily host
your notebooks on a Paas such as [Heroku][] or [Flynn][].

## Usage

If you're creating a new project on Heroku, use `--buildpack` to specify this
repository as your buildpack like this:

```console
heroku create --buildpack https://github.com/tswicegood/buildpack-notebook/
```

You can also add the buildpack to an existing application like this:

```console
heroku config:set BUILDPACK_URL=https://github.com/tswicegood/buildpack-notebook/
```


[conda]: http://conda.io/
[Flynn]: http://flynn.io/
[Heroku]: http://heroku.com/
[jupyter] https://jupyter.org/

Docker AWS CLI
==============

Docker image packaging for AWS CLI. This image is built on top of the
[official Python 2 Alpine image][1] to help keep it as light as possible, and is available on the
[Docker Hub][2].

Usage
-----

* The volume `/root/.aws` is exposed for mounting AWS configuration. You can set it up by mounting
this folder and running `docker run -it --rm -v "<HOST_CONF>:/root/.aws" seeruk/aws-cli configure`.
* The entrypoint of this image is set to `aws`, so you can just specify arguments to the AWS CLI
directly, e.g: `docker run -it --rm seeruk/aws-cli --version`.

License
-------

MIT

Contributing
------------

Feel free to open a [pull request][3], or file an [issue][4] on Github. I always welcome
contributions as long as they're for the benefit of all (potential) users of this image.

If you're unsure about anything, feel free to ask about it in an issue before you get your heart
set on fixing it yourself.

[1]: https://hub.docker.com/_/python
[2]: https://hub.docker.com/r/seeruk/aws-cli
[3]: https://github.com/SeerUK/docker-aws-cli/pulls
[4]: https://github.com/SeerUK/docker-aws-cli/issues

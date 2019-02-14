# Base Docker image for Django applications
Based on ideas from [jBoss base image](https://github.com/jboss-dockerfiles/base).

## What's included?
* Python 3.6 (based on Debian stretch)
* postgresql-client
* locales
* gettext (used for django compile messages)
* PIP (latest version)

## Ideas or best practices behind this image
* Run application server using an unpriviledged user.
* Make use of layered images.
[Read the full article here](https://developers.redhat.com/blog/2016/02/24/10-things-to-avoid-in-docker-containers/)

## How to use?
1. A user and group named django are created and available.
2. Home dir of django user and WORKDIR is set to /opt/django, use it to mount your code and other resources.

## Contributions
Feel free to submit issues and merge requests. :)

# heroku-buildpack-plenv

This heroku buildpack achieves the following:

1. Uses the application's `.perl_version` file to compile the required perl version via [plenv](https://github.com/tokuhirom/plenv).
1. Installs perl dependencies via [Carton](https://metacpan.org/pod/Carton).
1. Runs the application using [starman](https://metacpan.org/dist/Starman/view/script/starman).
1. Caches the above for quick deploys.

## Inspiration

Based on the excellent work by [Tatsuhiko Miyagawa](https://github.com/miyagawa):

https://github.com/miyagawa/heroku-buildpack-perl#carton


# Roadiz CMS pack for Symfony

This is a Flex pack to install Roadiz CMS.

Installation instructions are available in the [Roadiz documentation](https://docs.roadiz.io/en/v2.0.0/).

```shell
mkdir -p ./themes
mkdir -p ./var/secret

bin/console doctrine:migrations:migrate
bin/console themes:assets:install Rozier
bin/console install
```

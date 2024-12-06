# Roadiz CMS pack for Symfony

This is a Flex pack to install Roadiz CMS.

Installation instructions are available in the [Roadiz documentation](https://docs.roadiz.io/en/latest/).

If you want to start a new headless project with Roadiz, check https://github.com/roadiz/skeleton.

```shell
mkdir -p ./var/secret
mkdir -p ./var/export
mkdir -p ./public/assets
mkdir -p ./public/files

bin/console doctrine:migrations:migrate
bin/console themes:assets:install Rozier
bin/console install
```

Update your `composer.json` to autoload themes and generated entities

```json
{
    "autoload": {
        "psr-4": {
            "Themes\\": "themes/"
        }
    }
}
```

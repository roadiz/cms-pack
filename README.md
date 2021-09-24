# Roadiz CMS pack for Symfony

This is a Flex pack to install Roadiz CMS.

Installation instructions are available in the [Roadiz documentation](https://docs.roadiz.io/en/v2.0.0/).

```shell
mkdir -p ./themes
mkdir -p ./var/secret
mkdir -p ./public/assets
mkdir -p ./public/files
mkdir -p ./generated

bin/console doctrine:migrations:migrate
bin/console themes:assets:install Rozier
bin/console install
```

Update your `composer.json` to autoload themes and generated entities

```json
{
    "autoload": {
        "psr-4": {
            "Themes\\": "themes/",
            "GeneratedNodeSources\\": "generated/"
        }
    }
}
```

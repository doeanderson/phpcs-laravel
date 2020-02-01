
# phpcs-laravel configuration

## Global Installation

To globally install this custom standard along with `phpcs` and `phpcbf`, add the following to your `~/.composer/composer.json` file.

```json
"repositories": [
        {
            "type": "vcs",
            "url": "https://github.com/doeanderson/phpcs-laravel"
        }
    ],
```
Then run the following command.

```shell
composer global require doeanderson/phpcs-laravel
phpcs -i
```
You should now see the `phpcs-laravel` standard listed.

## Installation per project

Add the following to your project's `composer.json` file.
```json
"repositories": [
        {
            "type": "vcs",
            "url": "https://github.com/doeanderson/phpcs-laravel"
        }
    ],
```

Then run the following command.
```shell
composer require --dev doeanderson/phpcs-laravel
```
Copy the contents of `phpcs.xml.dist` from this repo to your project's root folder as `phpcs.xml`.

Now you may run `./vendor/bin/phpcs` to scan your entire project or `./vendor/bin/phpcbf` to automatically fix/beautify files.


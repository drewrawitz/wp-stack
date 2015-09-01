# Wordpress Boilerplate
This is a modern WordPress stack that helps you get started with the best development tools and project structure. This stack is heavily based on [Bedrock](https://github.com/roots/bedrock).

## Features

* Better folder structure
* Dependency management with [Composer](http://getcomposer.org)
* Easy WordPress configuration with environment specific files
* Environment variables with [Dotenv](https://github.com/vlucas/phpdotenv)
* Autoloader for mu-plugins (use regular plugins as mu-plugins)

## Requirements

* PHP >= 5.4
* Composer - [Install](https://getcomposer.org/doc/00-intro.md#installation-linux-unix-osx)

## Install with Ansible

Follow the [WP-Ansible Installation Instructions](https://github.com/drewrawitz/wp-ansible) and just clone this repo as the `site` folder.

## Standalone Install

1. Clone the git repo - `git clone https://github.com/drewrawitz/wp-stack.git`
2. Run `composer install`
3. Copy `.env.example` to `.env` and update environment variables:
  * `DB_NAME` - Database name
  * `DB_USER` - Database user
  * `DB_PASSWORD` - Database password
  * `DB_HOST` - Database host
  * `WP_ENV` - Set to environment (`development`, `staging`, `production`)
  * `WP_HOME` - Full URL to WordPress home (http://example.com)
  * `WP_SITEURL` - Full URL to WordPress including subdirectory (http://example.com/wp)
4. Add theme(s) in `web/app/themes` as you would for a normal WordPress site.
4. Set your site vhost document root to `/path/to/site/web/` (`/path/to/site/current/web/` if using deploys)
5. Access WP admin at `http://example.com/wp/wp-admin`

## Documentation

For more detailed documentation, go to the [Bedrock GitHub Page](https://github.com/roots/bedrock) or the [Bedrock Wiki](https://github.com/roots/bedrock/wiki).

![saplings](https://github.com/kanopi/saplings/assets/5177009/a6377e32-deb2-49d8-873a-f3dd5a36fa7c)

# Saplings - OpenID Login

Configures OpenID Connect for logging into Drupal using popular identity
providers.

## Overview

This recipe installs and configures the necessary modules and settings to enable
OpenID Connect authentication on a Drupal site. It supports a range of OpenID
providers, including Google, Facebook, GitHub, LinkedIn, Okta, and generic
OpenID services.

## Features
- The recipe asks which provider you want to set up, and your ID and secret.
- The recipe can be applied multiple times for setting up additional providers.

## Application

```
composer require kanopi/saplings-login-openid
drush recipe ../recipes/saplings-login-openid
```

### Configure OpenID Providers
Set up providers at the following URLs:

- Facebook - https://developers.facebook.com/apps/
- GitHub - https://github.com/settings/developers
- Google - https://console.developers.google.com
- LinkedIn - https://www.linkedin.com/developers/apps
- Okta - TBD

See also the module's documentation at https://www.drupal.org/node/2274339

## Usage

Authenticated users will then be able to choose to connect their accounts to
the providers you have set up from their user page.

# plesk_lock_promos

Ansible Playbook for disabling useless promos on plesk.

This playbook uses a docker runner to deploy settings to your plesk on linux installation to disalbe useless promo links and banners in your plesk setup.

## Usage

Modify test.yml and plesk.yml in the inventory folder.  We use test.yml for our test server. Changed settings will be tested before deploying to the production stage inventory in plesk.yml.
Make sure your gitlab runner can connect to all of your plesk servers, use ssh keys!
Tag your runner with "ansible" or change the tag in the .gitlab-ci.yml.

## What we install

- Enginx and http2 for best performance!

## What we disable

There are some things that can be disabled in the plesk config:

- Promo banners
- Plesk Twitter links
- Plesk Facebook links
- Plesk Rating links
- Plesk Tracking links
- sentry.io Tracking
- Hire a Developer in WP Toolkit
- Monitoring 360 Buttons
- Disable MyPlesk Login

# Features

If you know other things that can be disabled feel free to contact me via: te at powie dot de.

## Setup and Use

1. If you don't already, install drush 9 globally `composer global require drush/drush:^9.4.0`
2. Ensure drush alias files for the site to be audited are in you drush aliases (e.g., `~/.drush/sites/`). When using BLT, the aliases only live in the project root, so you may need to copy those over.
3. From the drutiny directory, run `./vendor/bin/drutiny profile:run d8_security_review <@your-sites-drush-alias> --uri=<domain of your site>`

## Known issues

1. The Unused Modules test is not working with D8/Drush 9.


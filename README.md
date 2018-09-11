
## Setup and Use
1. Install the project using `composer create-project ba66e77/drutinizeme:@dev audit_tools`
    - replace `audit_tools` with whatever name makes you happy
2. If you don't already, install drush 9 globally `composer global require drush/drush:^9.4.0`
3. Ensure drush alias files for the site to be audited are in you drush aliases (e.g., `~/.drush/sites/`). 
    - When using [BLT](https://github.com/acquia/blt), the aliases only live in the project root, so you may need to copy those over.
4. From the audit_tools directory (or whatever you named it in step 1), run `./vendor/bin/drutiny profile:run d8_security_review <@your-sites-drush-alias> --uri=<domain of your site>`
    - Too see what other profiles are available, run `./vendor/bin/drutiny profile:list`

## Known issues

1. The Unused Modules test is not working with D8/Drush 9.


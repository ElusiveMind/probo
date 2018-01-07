# Probo Changelog

## 3.11.4
 - Dec 6 2017
 - Provide db prefix settings to the Wordpress plugin (see: https://github.com/ProboCI/probo/pull/133)

## 3.11.3
 - Nov 20 2017
 - Update list of docker images to be allowed for builds (see: https://github.com/ProboCI/probo/pull/130)
 - Fixing a bug in the way PHP ini settings are managed (see: https://github.com/ProboCI/probo/pull/121)
 - Allow for custom Wordpress database table prefixes (see: https://github.com/ProboCI/probo/pull/116)
 - Auto-testing and linting with git pull or pushes

## 3.11.2
 - Nov 16 2017
 - Linting code to keep up standards
 - Adding nightly images to our whitelist of docker images allowed for builds (see: https://github.com/ProboCI/probo/pull/129)
 - Update tests to prevent undefined probo yaml options (see: https://github.com/ProboCI/probo/pull/128)

## 3.11.1
 - Nov 13 2017
 - Add option to provide Drupal with a database prefix (see: https://github.com/ProboCI/probo/pull/126)

## 3.11.0
 - Nov 10 2017
 - Remove `-e` from bash args for build plugins to allow bash runs to continue if something failes (see: https://github.com/ProboCI/probo/pull/77)
 - Address incompatible buildId and Container stop (see: https://github.com/ProboCI/probo/pull/124)

## 3.10.0
 - Jun 12 2017
 - Applies a fix that caused the container manager to crash in some scenarios.
 - Adds new allowed docker images to the default configuration.

## 3.9.0
 - Add branch link & name, PR link & name, and commit link to ENV. These are now accessible in ENV variables. (including from within .probo.yaml)
 - See the docs for more info on ENV variables: https://docs.probo.ci/build/steps

## 3.8.0
 - Use constants to define status / state of builds and build steps
 - Create a new 'running' state for builds and build steps that are in progress. From now on, a 'pending' state means the build or build step is saved but not yet started.
 - Map the 'running' state to 'pending' for Github updates, because Github does not recognize a state called 'running'.

## v3.1.2

 - Added ability to specify the Drupal 8 configuration directory from which data should be synchronized.

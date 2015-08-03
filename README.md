## About

This project utilizes the [pantheon-systems/circle-scripts](https://github.com/pantheon-systems/circle-scripts) project in order to create a project that can be used to test updates to the [drops-7](https://github.com/patheon-systems/drops-7) project.

New releases on drops-7 are accompanied by a PR on this project that points the Composer project pantheon-systems/drops-7 at the branch in the drops-7 repository to be tested.  This PR is not intended to ever be merged; it should be deleted once it has finished running. Once the new drops-7 branch is merged in to master, then the master branch of this repository (updates-7) will still point to it, and only a "composer update" should be needed.

n.b. Drops-7 must be registered in Packagist, and the composer.json file must be updated once this is done.  This change will also require changes to the scripts in [pantheon-systems/downstream-updater](https://github.com/pantheon-systems/downstream-updater).

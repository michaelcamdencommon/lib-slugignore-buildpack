# Heroku Slugignore Buildpack

Heroku provides functionality to ignore files at the root level via the .slugignore file. Unfortunately it executes the removal of those files before buildpacks are executed so we don't have a chance to build our apps.

This buildpack will read from the text file specified at the SLUGIGNORE variable, and delete the associated folders.

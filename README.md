# Actions

This project includes reusbale workflows for building and deploying Drupal sites to Acquia, Pantheon, and Platform.

## Usage
It's recommended to use these actions with Paragon Base. 

## Workflows
### build_deploy
Installs project dependencies and builds the theme. Then deploy the artifact to a hosting platform.
### deploy
Pushes current repository state to a hosting platform

## Actions
### actions (WIP)
Contains the pre_build and post_deploy actions. These actions call other actions specific to each hosting provider
### pantheon
Contains the actual pre_build and post_deploy steps

## Development
````
act workflow_dispatch -P ubuntu-latest=shivammathur/node:latest --secret-file .secrets --env-file .env --var-file .vars
````
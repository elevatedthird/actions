# Actions

This project includes reusbale workflows for building and deploying Drupal sites to Acquia, Pantheon, and Platform.

## Usage
It's recommended to use these actions with Paragon Base.
You must have the following secrets in your GH repo:
- `SSH_PASSPHRASE`
- `SSH_PRIVATE_KEY`
These are added to each repo at an organization level, but can be overriden. You must invite the hosting@elevaedthird account to the project's
hosting platform so the key can access the project

## ENV file
Paragon comes with a .env file in the project root with variables for these workflows

## Workflows
### build_deploy
Installs project dependencies and builds the theme. Then deploy the artifact to a hosting platform.

## Composite Actions
### ssh-agent
Contains an action for starting the SSH Agent to connect to the remote host

### pantheon
Contains the actual pre_build and post_deploy steps

### test-php (WIP)
Contains an action for testing the project with phpcs ad phpstan.

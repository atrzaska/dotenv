# Dotenv

Dotenv is a application to load your dotenv files from current working directory into environment and provide environment variables to other programs.

The software was designed to help load environment variables in Rails applications, but is not limited to Rails.

## Examples:

Add environment variables in the `.env` files of your project

    touch .env
    touch .env.test
    touch .env.development
    touch .env.preview
    touch .env.staging
    touch .env.production
    touch .env.local

Run your software

    dotenv env
    dotenv test bundle exec rspec
    dotenv bundle exec rails s
    dotenv exec env
    dotenv -f my_custom_env_file exec env
    dotenv -f my_custom_env_file env

# Requirements

- Ruby (Tested on 2.5.1)

# Setup

The setup is as simple as downloading the binary

    wget https://raw.githubusercontent.com/andrzejtrzaska/dotenv/master/dotenv
    chmod +x dotenv
    ./dotenv


Ideally you should add dotenv to your PATH environment variable or move it to some location in PATH. That will make using the program a lot easier.

You can also create some aliases to avoid typing dotenv every time.

    alias be='dotenv bundle exec'

# Environment integrations

Dotenv uses `RAILS_ENV` or `ENV` environment variable to load correct environment file.

For example for `RAILS_ENV=development` or `ENV=development` it will load in order:

- `.env`
- `.env.development`
- `.env.local`

Default environment is `development`.

# Notes

Unlike normal dotenv, it is possible to override already set environment variables.

# Licence

MIT

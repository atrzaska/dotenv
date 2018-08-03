# Dotenv

Dotenv is a application to load your dotenv files from current working directory into environment and provide environment variables to other programs.

## Examples:

Add environment variables in the env viles of your project

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

# Requirements

- Ruby (Tested on 2.5.1)

# Setup

The setup is as simple as downloading the binary

    wget https://raw.githubusercontent.com/andrzejtrzaska/dotenv/master/dotenv
    chmod +x dotenv
    ./dotenv


Ideally you should add dotenv to your PATH env var or move it to some location in PATH. That will make using the program a lot easier.

You can also create some aliases to avoid typing dotenv every time.

    alias be='dotenv bundle exec'

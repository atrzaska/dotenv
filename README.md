# Dotenv

Dotenv is a application to load your dotenv files from current working directory into environment and provide environment variables to other programs.

Examples:

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

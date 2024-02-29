# RAPID

Minimal Rails edge setup, using esbuild, tailwindcss and postgresql.

## Getting started

### Initial application setup

Run the setup script that will run the needed setup steps for the application, installing all gems and packages, database preparing etc.

```sh
bin/setup
```

### Development

Will run [Overmind](https://github.com/DarthSim/overmind) (or Foreman if Overmind is not installed), starts the build for all assets automaticly and will start the rails server.

```sh
bin/dev
```

## Code Guidelines

It uses [Rails Omakase RuboCop](https://github.com/rails/rubocop-rails-omakase) for Ruby to automatically fix code style offenses.

```sh
bin/rubocop
```

to automatically format Ruby with Rubocop you can run:

```sh
bin/rubocop -a
```

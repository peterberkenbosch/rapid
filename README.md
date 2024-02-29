# RAPID

Minimal Rails edge setup, using esbuild, tailwindcss and postgresql.

You need the following installed:
* Ruby >= 3.2.0 (`asdf install`)
* Bundler (`gem install bundler`)
* Node 20 (`asdf install`)
* Yarn (`npm install yarn --global`)
* Postgresql 14 (`brew install postgresql@16` start with: `brew services start postgresql@16`)
* Redis (`brew install redis` start with: `brew services start redis`)

Optional:
* Overmind (`brew install tmux overmind`)

If you are using [asdf](https://asdf-vm.com/) (I recommend that you do :) ) you can install the required Ruby and NodeJS versions with `asdf install`

The Homebrew dependencies can be installed with running:

```bash
brew bundle install --no-upgrade
```

Additional Homebrew dependencies can be added to the `Brewfile`

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

## Additional Installed Gems:
* [Annotate, Add a comment summarizing the current schema](https://github.com/ctran/annotate_models)
* [Strong Migrations, Catch unsafe migrations in development](https://github.com/ankane/strong_migrations)

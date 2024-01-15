# [Backstage](https://backstage.io)

This is your newly scaffolded Backstage App, Good Luck!

To start the app, run:

```sh
yarn install
yarn dev
```

Configuration

Install Postgress
```sh
brew install postgresql@15
echo 'export PATH="/opt/homebrew/opt/postgresql@15/bin:$PATH"' >> ~/.zshrc
source ~/.zshrc
```


Template creation
```sh
yarn add --cwd packages/backend pg
```

Note: if you're running Backstage with Node 20 or later, you'll need to pass the flag --no-node-snapshot to Node in order to use the templates feature. One way to do this is to specify the NODE_OPTIONS environment variable before starting Backstage: export NODE_OPTIONS=--no-node-snapshot

Create .env file in the root of the project

```
POSTGRES_HOST=localhost
POSTGRES_PORT=5432 
POSTGRES_USER=<your_username>
POSTGRES_PASSWORD=secret
AUTH_GITHUB_CLIENT_ID=2b28145f2873f62cda86
AUTH_GITHUB_CLIENT_SECRET=0e0a1cc62ddef67aa4c05f5975c59c706585e92b
GITHUB_TOKEN=<github_token>
```
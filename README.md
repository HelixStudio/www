# www

A monorepo with shell scripts to ease the deployment of Helix on custom servers.

Included web services:

- helix: the main website (port 3000)
- exec: the code execution server (port 5000)
- ctf-server: the management server for ctf challenges (port 8000)

## setup

Clone the repo:

```sh
git clone https://github.com/helixstudio/www --recursive
```

Create the `.env` file, based on the structure of `.env.example`.

```sh
cp .env ./services/helix/.env
```

Run the docker services:

```sh
docker compose up -d
```

And to stop:

```sh
docker compose stop
```

# update

```sh
git submodule update --remote --merge
```

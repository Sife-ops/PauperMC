# PauperMC

## Usage

```yaml
local:
  hosts:
    localhost:
      ansible_connection: local

paupermc:
  hosts:
    "123.123.123.123":
```

You can quickly create a minecraft server

```bash
./paupermc-start.yml
```

and backup your world

```bash
./paupermc-backup.yml
```

At this point you may want to delete the server (to save money when you're not
using it). Later on you can make a new server and run

```bash
./paupermc-start.yml -e "{restore: true}"
```

Only takes about 10 mins to start up on gud dale up.

## Examples

```bash
docker exec -i mc rcon-cli
```

```bash
./paupermc-start.yml -e "{seed: '123456'}"
```

## Reference

- https://docker-minecraft-server.readthedocs.io/

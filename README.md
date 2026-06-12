# Maintainerr Unraid Templates

Official [Unraid Community Applications](https://unraid.net/community/apps) templates, maintained by the [Maintainerr](https://github.com/Maintainerr/Maintainerr) team.

## Apps

| App         | Template                                               | Image                                    |
| ----------- | ------------------------------------------------------ | ---------------------------------------- |
| Maintainerr | [templates/maintainerr.xml](templates/maintainerr.xml) | `ghcr.io/maintainerr/maintainerr:latest` |

## Installation

Install **Maintainerr** from the **Apps** tab in the Unraid web UI. The defaults work out of the box:

- **WebUI**: port `6246`
- **Data**: `/mnt/user/appdata/maintainerr` (holds the database and logs)
- **Timezone**: set this to your local timezone so rule schedules run when you expect

The container runs as user `1000:1000`. Before the first start, fix the appdata ownership in the Unraid terminal (adjust if you changed the appdata path):

```sh
chown -R 1000:1000 /mnt/user/appdata/maintainerr
```

To try unreleased changes, switch the release branch from **Stable releases** to the **development** tag in the template.

## Support

- [Documentation](https://docs.maintainerr.info)
- [Discord](https://discord.maintainerr.info)
- [GitHub issues](https://github.com/Maintainerr/Maintainerr/issues)

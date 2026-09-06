# Next Door Photos

This repository holds the public organization profile for
[github.com/Next-Door-Photos](https://github.com/Next-Door-Photos).

| What | Where |
|---|---|
| Profile page shown on the org home | [`profile/README.md`](profile/README.md) |
| Org settings (description, website, location) | [`org-profile.json`](org-profile.json), applied with [`scripts/apply-org-profile.sh`](scripts/apply-org-profile.sh) |

## Organization settings

GitHub keeps an organization's description, website, and location in org
settings rather than in a repository, so this repo records the intended values
and ships a script that applies them.

| Field | Value |
|---|---|
| Display name | Next Door Photos |
| Description | Real estate media without the wait. Same day booking, next day delivery, from local owners across 100+ North American territories. Certified B Corp. |
| Website | https://nextdoorphotos.com |
| Location | Zeeland, MI |

To apply, an org owner runs the following from a machine with an authenticated
[GitHub CLI](https://cli.github.com):

```sh
./scripts/apply-org-profile.sh --dry-run   # preview
./scripts/apply-org-profile.sh             # apply
```

Edit `org-profile.json` first when the values need to change, then re-run the
script so the repo and the org settings stay in step.

# Ansible Playbooks

These are Ansible playbooks that I use or have used in the past.
They may work or they may not. (They most likely did at one point in time.)

Use with caution and at your own risk.

## Development

Linting and hooks are managed by [pre-commit](https://pre-commit.com/) (see `.pre-commit-config.yaml`). CI uses [pre-commit.ci](https://pre-commit.ci/):

- **One-time setup:** Install the [pre-commit.ci GitHub App](https://github.com/apps/pre-commit-ci) on this repository (Sign in at [pre-commit.ci](https://pre-commit.ci/) and add the app to the repo).
- **Locally:** Run `pre-commit install`, then `pre-commit run --all-files` to check everything.
- **In CI:** pre-commit.ci runs on pull requests, can auto-fix commits, and runs weekly hook autoupdates.

## Example usage

```bash
ansible-navigator run -m stdout playbooks/cloud_cli_update.yml
```

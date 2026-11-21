# GateDisclose

I'm Desmond, a platform/DevOps person who hoards small scripts until they become a toolbox. If a task has been run twice, I'm already writing the wrapper for it.

## Usually building
- Idempotent shell scripts for things that should have been one command.
- Pipeline glue, deploy helpers, and backup checks.
- Log triage with `rg`, `jq`, and low expectations.
- Runbooks that actually match the system.

## Current learning
Go, for the CLIs that outgrew bash. Also making my Ansible a bit less haunted.

```bash
#!/usr/bin/env bash
set -euo pipefail

# if this looks disposable, it probably touches production
main() {
  echo "checking the thing before automating the thing"
}

main "$@"
```

## Around the repos
Mostly small utilities: cron cleanup, incident notes to checks, container build helpers, and infra glue. If you find one of these scripts in the wild, open an issue before it becomes a cron job.

![GitHub stats](https://github-readme-stats.vercel.app/api?username=GateDisclose&show_icons=true&theme=tokyonight&hide_border=true&border_radius=8)
![Top languages](https://github-readme-stats.vercel.app/api/top-langs/?username=GateDisclose&layout=compact&theme=tokyonight&hide_border=true&border_radius=8)
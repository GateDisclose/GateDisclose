# GateDisclose

I'm Paolina, a DevOps engineer with a script hoarding problem. I keep the one-off fixes, name them after the incident, and turn the useful ones into gates that say no before prod does.

![GitHub stats](https://github-readme-stats.vercel.app/api?username=heckbertpaolina&show_icons=true&hide_rank=true&theme=tokyonight&title_color=7aa2f7&icon_color=bb9af7&text_color=c0caf5&bg_color=1a1b26&border_radius=8&hide_border=true)
![Top languages](https://github-readme-stats.vercel.app/api/top-langs/?username=heckbertpaolina&layout=compact&theme=tokyonight&title_color=7aa2f7&icon_color=bb9af7&text_color=c0caf5&bg_color=1a1b26&border_radius=8&hide_border=true)

## The hoard
Shell scripts, dotfiles, cron wrappers, rollback notes, and a growing folder called `maybe-useful`. If it ran twice, it gets a README and a test.

## What I build
Deploy pipelines that fail early and explain themselves. Terraform plan checks, secrets scans, OPA/Rego policies, and small CLIs that make on-call less archaeological.

## Reusable gate
```bash
#!/usr/bin/env bash
set -euo pipefail
find scripts -name '*.sh' -print0 | xargs -0 shellcheck
git diff --exit-code -- .github/workflows
```

## Currently learning
How to write less bash and more Rego, plus making reusable GitHub Actions that are not a haunted house of inputs.
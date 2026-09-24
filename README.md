# Odyssey Playtest

Public browser build of **Odyssey** used for mobile and external playtesting.

The game source code remains in the private `odyssey-homeward-survival` repository. This repository contains only the deployment workflow and deployment metadata; GitHub Pages receives the compiled `dist/` artifact generated from `feature/odyssey-vertical-slice`.

Playtest URL once GitHub Pages is enabled and the source token is configured:

https://ram8o211.github.io/odyssey-playtest/

## Deployment

The scheduled workflow checks the private Odyssey branch every five minutes. It rebuilds and deploys only when the source commit changes. Public builds use `PUBLIC_PLAYTEST=1`, which disables source maps.

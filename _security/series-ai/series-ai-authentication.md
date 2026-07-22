---
api_key_in: []
auth_types: []
description: RUN.world is the only supported auth system for a game. The platform signs players in and hands the game their identity; games cannot run their own login. Programmatic/CLI access uses per-game opaque API keys.
kind: authentication
layout: security
method: searched
name: Series Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Series AI declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Series AI
provider_slug: series-ai
scheme_count: 0
schemes: []
slug: series-ai-authentication
source_filename: series-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://github.com/series-ai/venus-sdk-docs (runtime-environment.md, deploying-your-game.md, api/ACCESS_GATE.md, api/PROFILE.md, api/APP.md)\nname: RUN.world Authentication\ndescription: >-\n  RUN.world is the only supported auth system for a game. The platform signs\n  players in and hands the game their identity; games cannot run their own\n  login. Programmatic/CLI access uses per-game opaque API keys.\nplayer_identity:\n  model: platform-provided\n  detail: >-\n    RUN.world authenticates players and passes identity to the game. Self-hosted\n    Firebase Auth, Google/Apple/third-party OAuth, and custom identity providers\n    do not work inside the game iframe (auth scripts, token endpoints, and OAuth\n    popups are blocked by the platform sandbox).\n  apis:\n  - name: Access Gate API\n    purpose: Require sign-in / gate features behind a signed-in player.\n    ref: rundot-developer-platform/api/ACCESS_GATE.md\n  - name:\
  \ Profiles API\n    purpose: Read the signed-in player's identity.\n    ref: rundot-developer-platform/api/PROFILE.md\n  - name: App API\n    purpose: Check the player's role for the game (owner/editor).\n    ref: rundot-developer-platform/api/APP.md\nprogrammatic_access:\n  interactive:\n    scheme: browser login (Google account) via `rundot login`\n    session: stored locally in ~/.rundot/ (macOS/Linux) or %USERPROFILE%\\.rundot\\ (Windows)\n  api_key:\n    scheme: bearer-style per-game API key\n    prefix: \"rk_\"\n    scope: single game; managed only by the game owner\n    lifecycle: \"rundot game api-keys create|list|regenerate|revoke; --expires-in-days supported\"\n    display: \"secret printed once on create/regenerate — save immediately\"\n    restriction: >-\n      Key management is unavailable when authenticated with an rk_ key; it\n      requires an interactive owner login. Some prod-only tooling also rejects\n      rk_ sessions.\n    use: \"headless CI/CD (GitHub Actions, GitLab\
  \ CI): `rundot login --api-key rk_...`\"\nsecurity_schemes:\n- type: platform-managed (player)\n  location: RUN.world host\n- type: apiKey\n  name: rk_ per-game key\n  in: cli/ci session\noauth2: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/series-ai/refs/heads/main/authentication/series-ai-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Games
- Game Development
- Artificial Intelligence
- Generative AI
- Game Engine
- SDK
- Developer Tools
- Multiplayer
- HTML5
---

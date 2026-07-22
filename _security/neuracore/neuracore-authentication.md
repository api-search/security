---
api_key_in:
- header
- env
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Neuracore Authentication
name_suffix: Authentication
oauth_flows: []
overview: Neuracore secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Neuracore
provider_slug: neuracore
scheme_count: 2
schemes:
- env: NEURACORE_API_KEY
  key_prefix: nrc_
  name: NeuracoreApiKey
  obtain: Run `neuracore login` (interactive or --email/--password) which authenticates and stores an API key at ~/.neuracore/config.json, or set NEURACORE_API_KEY.
  sources:
  - docs/environment_variable.md
  - neuracore/core/cli/generate_api_key.py
  type: apiKey
- detail: Interactive account login backed by requests-oauthlib; exchanges account credentials for a session/API key used by the SDK and CLI.
  name: NeuracoreLogin
  sources:
  - neuracore/core/auth.py
  type: oauth2
slug: neuracore-authentication
source_filename: neuracore-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://github.com/NeuracoreAI/neuracore/blob/main/docs/environment_variable.md\ndocs: https://github.com/NeuracoreAI/neuracore/blob/main/docs/commandline.md\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [header, env]\n  api_key_prefix: nrc_\n  notes: >-\n    No public OpenAPI document is published; the authentication model is captured\n    from the SDK/CLI documentation and source (requests-oauthlib login flow +\n    API-key header auth against api.neuracore.com/api).\nschemes:\n- name: NeuracoreApiKey\n  type: apiKey\n  key_prefix: nrc_\n  env: NEURACORE_API_KEY\n  obtain: >-\n    Run `neuracore login` (interactive or --email/--password) which authenticates\n    and stores an API key at ~/.neuracore/config.json, or set NEURACORE_API_KEY.\n  sources: [docs/environment_variable.md, neuracore/core/cli/generate_api_key.py]\n- name: NeuracoreLogin\n  type: oauth2\n  detail: >-\n    Interactive account login backed by requests-oauthlib;\
  \ exchanges account\n    credentials for a session/API key used by the SDK and CLI.\n  sources: [neuracore/core/auth.py]\norg_context:\n  env: NEURACORE_ORG_ID\n  format: uuid\n  note: >-\n    Requests are scoped to an organization; select with `neuracore select-org`\n    or set NEURACORE_ORG_ID.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/neuracore/refs/heads/main/authentication/neuracore-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Robotics
- Robot Learning
- Machine Learning
- Imitation Learning
- Reinforcement Learning
- Teleoperation
- Artificial Intelligence
- SDK
- Python
---

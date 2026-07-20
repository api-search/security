---
api_key_in:
- header
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Ellipsis Authentication
name_suffix: Authentication
oauth_flows:
- deviceCode
overview: Ellipsis secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the deviceCode flow(s).
provider_name: Ellipsis
provider_slug: ellipsis
scheme_count: 2
schemes:
- description: 'REST API requests authenticate with a bearer token created in the dashboard under Platform -> API keys (token format `ellipsis_key_...`), passed as `Authorization: Bearer <token>`. Requests without valid authorization return HTTP 401. In scripts/CI the token is supplied via the `ELLIPSIS_API_TOKEN` environment variable.'
  env: ELLIPSIS_API_TOKEN
  format: Bearer
  header: Authorization
  location: header
  name: bearerToken
  scheme: bearer
  type: http
- description: 'The `agent` CLI authenticates interactively via a device-code flow (`agent login`): it opens a verification URL in the browser and stores a user token at ~/.config/ellipsis/config.json.'
  flow: deviceCode
  name: deviceCodeLogin
  type: oauth2
  used_by: cli
slug: ellipsis-authentication
source_filename: ellipsis-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://www.ellipsis.dev/docs/reference/api\ndocs: https://www.ellipsis.dev/docs/reference/api\nsummary:\n  types: [http, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [deviceCode]\nschemes:\n- name: bearerToken\n  type: http\n  scheme: bearer\n  description: >-\n    REST API requests authenticate with a bearer token created in the dashboard\n    under Platform -> API keys (token format `ellipsis_key_...`), passed as\n    `Authorization: Bearer <token>`. Requests without valid authorization return\n    HTTP 401. In scripts/CI the token is supplied via the `ELLIPSIS_API_TOKEN`\n    environment variable.\n  location: header\n  header: Authorization\n  format: Bearer\n  env: ELLIPSIS_API_TOKEN\n- name: deviceCodeLogin\n  type: oauth2\n  flow: deviceCode\n  description: >-\n    The `agent` CLI authenticates interactively via a device-code flow\n    (`agent login`): it opens a verification URL in the browser and stores a\n  \
  \  user token at ~/.config/ellipsis/config.json.\n  used_by: cli\nsession_credentials:\n  note: >-\n    Each agent session additionally receives its own short-lived credentials —\n    a GitHub token scoped to the permissions/repos granted at install, a\n    synthetic API key, and a session-scoped token — all revoked at teardown\n    (least privilege). Sandbox tokens are denied privileged operations (HTTP 403).\nscopes: none-documented\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ellipsis/refs/heads/main/authentication/ellipsis-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Code Review
- AI Agents
- Coding Agents
- Developer Tools
- Software Development
- Automation
- DevOps
- Pull Requests
---

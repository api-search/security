---
anonymous_access: false
api_key_in: []
api_specs:
- filename: usewrit-app-agent-api-openapi.yml
  format: yaml
  label: usewrit-app Agent API
  slug: usewrit-app-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usewrit-app/openapi/usewrit-app-agent-api-openapi.yml
- filename: usewrit-app-automations-api-openapi.yml
  format: yaml
  label: usewrit-app Automations API
  slug: usewrit-app-automations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usewrit-app/openapi/usewrit-app-automations-api-openapi.yml
- filename: usewrit-app-cloud-api-openapi.yml
  format: yaml
  label: usewrit-app Cloud API
  slug: usewrit-app-cloud-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usewrit-app/openapi/usewrit-app-cloud-api-openapi.yml
- filename: usewrit-app-crawl-api-openapi.yml
  format: yaml
  label: usewrit-app Crawl API
  slug: usewrit-app-crawl-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usewrit-app/openapi/usewrit-app-crawl-api-openapi.yml
- filename: usewrit-app-data-api-openapi.yml
  format: yaml
  label: usewrit-app Data API
  slug: usewrit-app-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usewrit-app/openapi/usewrit-app-data-api-openapi.yml
- filename: usewrit-app-datasets-api-openapi.yml
  format: yaml
  label: usewrit-app Datasets API
  slug: usewrit-app-datasets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usewrit-app/openapi/usewrit-app-datasets-api-openapi.yml
- filename: usewrit-app-extractors-api-openapi.yml
  format: yaml
  label: usewrit-app Extractors API
  slug: usewrit-app-extractors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usewrit-app/openapi/usewrit-app-extractors-api-openapi.yml
- filename: usewrit-app-files-api-openapi.yml
  format: yaml
  label: usewrit-app Files API
  slug: usewrit-app-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usewrit-app/openapi/usewrit-app-files-api-openapi.yml
- filename: usewrit-app-keys-api-openapi.yml
  format: yaml
  label: usewrit-app Keys API
  slug: usewrit-app-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usewrit-app/openapi/usewrit-app-keys-api-openapi.yml
- filename: usewrit-app-monitors-api-openapi.yml
  format: yaml
  label: usewrit-app Monitors API
  slug: usewrit-app-monitors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usewrit-app/openapi/usewrit-app-monitors-api-openapi.yml
- filename: usewrit-app-personas-api-openapi.yml
  format: yaml
  label: usewrit-app Personas API
  slug: usewrit-app-personas-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usewrit-app/openapi/usewrit-app-personas-api-openapi.yml
- filename: usewrit-app-runs-api-openapi.yml
  format: yaml
  label: usewrit-app Runs API
  slug: usewrit-app-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usewrit-app/openapi/usewrit-app-runs-api-openapi.yml
- filename: usewrit-app-secrets-api-openapi.yml
  format: yaml
  label: usewrit-app Secrets API
  slug: usewrit-app-secrets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usewrit-app/openapi/usewrit-app-secrets-api-openapi.yml
- filename: usewrit-app-selectors-api-openapi.yml
  format: yaml
  label: usewrit-app Selectors API
  slug: usewrit-app-selectors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usewrit-app/openapi/usewrit-app-selectors-api-openapi.yml
- filename: usewrit-app-vault-api-openapi.yml
  format: yaml
  label: usewrit-app Vault API
  slug: usewrit-app-vault-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usewrit-app/openapi/usewrit-app-vault-api-openapi.yml
- filename: usewrit-app-workflows-api-openapi.yml
  format: yaml
  label: usewrit-app Workflows API
  slug: usewrit-app-workflows-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usewrit-app/openapi/usewrit-app-workflows-api-openapi.yml
- filename: usewrit-app-ws-ticket-api-openapi.yml
  format: yaml
  label: usewrit-app Ws Ticket API
  slug: usewrit-app-ws-ticket-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usewrit-app/openapi/usewrit-app-ws-ticket-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: usewrit-app Authentication
name_suffix: Authentication
oauth_flows: []
overview: usewrit-app secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: usewrit-app
provider_slug: usewrit-app
scheme_count: 1
schemes:
- description: "Every route (including `/v1/agent` and `/v1/health`) requires\n`Authorization: Bearer <token>`. Token families:\n\n- `wlt_…` — the runtime token from `runtime.json` (full access, used by the desktop\n  UI and SDK discovery).\n- `wlk_…` — a scoped API key minted via `POST /v1/keys` (CSV scopes `read|run|admin`;\n  `/v1/keys` itself requires the full-access token).\n- `wlo_…` — an OAuth 2.1 access token fr"
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/writ-agent.yaml
  type: http
slug: usewrit-app-authentication
source_filename: usewrit-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: derived\nsource: openapi/writ-agent.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: |-\n    Every route (including `/v1/agent` and `/v1/health`) requires\n    `Authorization: Bearer <token>`. Token families:\n\n    - `wlt_…` — the runtime token from `runtime.json` (full access, used by the desktop\n      UI and SDK discovery).\n    - `wlk_…` — a scoped API key minted via `POST /v1/keys` (CSV scopes `read|run|admin`;\n      `/v1/keys` itself requires the full-access token).\n    - `wlo_…` — an OAuth 2.1 access token fr\n  sources:\n  - openapi/writ-agent.yaml\n"
source_yaml_url: https://artifacts.apis.io/usewrit-app/authentication/usewrit-app-authentication.yml
summary_line: http · 1 scheme
tags:
- Automation
- MCP
- No-Code
- Software-as-a-Service
---

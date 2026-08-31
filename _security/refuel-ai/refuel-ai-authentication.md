---
api_key_in:
- header
api_specs:
- filename: refuel-ai-applications-api-openapi.yml
  format: yaml
  label: Refuel Applications API
  slug: refuel-ai-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refuel-ai/refs/heads/main/openapi/refuel-ai-applications-api-openapi.yml
- filename: refuel-ai-access-api-openapi.yml
  format: yaml
  label: Refuel Access API
  slug: refuel-ai-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refuel-ai/refs/heads/main/openapi/refuel-ai-access-api-openapi.yml
- filename: refuel-ai-csp-reports-api-openapi.yml
  format: yaml
  label: Refuel Csp Reports API
  slug: refuel-ai-csp-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refuel-ai/refs/heads/main/openapi/refuel-ai-csp-reports-api-openapi.yml
- filename: refuel-ai-datasets-api-openapi.yml
  format: yaml
  label: Refuel Datasets API
  slug: refuel-ai-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refuel-ai/refs/heads/main/openapi/refuel-ai-datasets-api-openapi.yml
- filename: refuel-ai-finetuned-models-api-openapi.yml
  format: yaml
  label: Refuel Finetuned Models API
  slug: refuel-ai-finetuned-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refuel-ai/refs/heads/main/openapi/refuel-ai-finetuned-models-api-openapi.yml
- filename: refuel-ai-integrations-api-openapi.yml
  format: yaml
  label: Refuel Integrations API
  slug: refuel-ai-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refuel-ai/refs/heads/main/openapi/refuel-ai-integrations-api-openapi.yml
- filename: refuel-ai-labs-api-openapi.yml
  format: yaml
  label: Refuel Labs API
  slug: refuel-ai-labs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refuel-ai/refs/heads/main/openapi/refuel-ai-labs-api-openapi.yml
- filename: refuel-ai-models-api-openapi.yml
  format: yaml
  label: Refuel Models API
  slug: refuel-ai-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refuel-ai/refs/heads/main/openapi/refuel-ai-models-api-openapi.yml
- filename: refuel-ai-projects-api-openapi.yml
  format: yaml
  label: Refuel Projects API
  slug: refuel-ai-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refuel-ai/refs/heads/main/openapi/refuel-ai-projects-api-openapi.yml
- filename: refuel-ai-refuel-cloud-api-api-openapi.yml
  format: yaml
  label: Refuel Refuel Cloud API
  slug: refuel-ai-refuel-cloud-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refuel-ai/refs/heads/main/openapi/refuel-ai-refuel-cloud-api-api-openapi.yml
- filename: refuel-ai-schema-api-openapi.yml
  format: yaml
  label: Refuel Schema API
  slug: refuel-ai-schema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refuel-ai/refs/heads/main/openapi/refuel-ai-schema-api-openapi.yml
- filename: refuel-ai-tasks-api-openapi.yml
  format: yaml
  label: Refuel Tasks API
  slug: refuel-ai-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refuel-ai/refs/heads/main/openapi/refuel-ai-tasks-api-openapi.yml
- filename: refuel-ai-team-api-openapi.yml
  format: yaml
  label: Refuel Team API
  slug: refuel-ai-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refuel-ai/refs/heads/main/openapi/refuel-ai-team-api-openapi.yml
- filename: refuel-ai-teams-api-openapi.yml
  format: yaml
  label: Refuel Teams API
  slug: refuel-ai-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refuel-ai/refs/heads/main/openapi/refuel-ai-teams-api-openapi.yml
- filename: refuel-ai-usage-api-openapi.yml
  format: yaml
  label: Refuel Usage API
  slug: refuel-ai-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refuel-ai/refs/heads/main/openapi/refuel-ai-usage-api-openapi.yml
- filename: refuel-ai-user-api-openapi.yml
  format: yaml
  label: Refuel User API
  slug: refuel-ai-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refuel-ai/refs/heads/main/openapi/refuel-ai-user-api-openapi.yml
- filename: refuel-ai-users-api-openapi.yml
  format: yaml
  label: Refuel Users API
  slug: refuel-ai-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refuel-ai/refs/heads/main/openapi/refuel-ai-users-api-openapi.yml
- filename: refuel-ai-webhook-api-openapi.yml
  format: yaml
  label: Refuel Webhook API
  slug: refuel-ai-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refuel-ai/refs/heads/main/openapi/refuel-ai-webhook-api-openapi.yml
- filename: refuel-ai-webhooks-api-openapi.yml
  format: yaml
  label: Refuel Webhooks API
  slug: refuel-ai-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refuel-ai/refs/heads/main/openapi/refuel-ai-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Refuel Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Refuel secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Refuel
provider_slug: refuel-ai
scheme_count: 2
schemes:
- applied_to: 99 of 108 operations in the Cloud API spec declare a HTTPBearer security requirement
  description: 'A Refuel API key sent as an HTTP Bearer token: `Authorization: Bearer <REFUEL_API_KEY>`. One key per team; it is issued in the Refuel app. Refuel''s own catalog documentation shows it in use against the label endpoint, and the Python SDK reads it from the REFUEL_API_KEY environment variable (or an `api_key` init option).'
  name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/refuel-ai-cloud-api-openapi.yml
  - openapi/refuel-ai-applications-api-openapi.yml
  - https://docs.refuel.ai/sdk/python
  type: http
- alias_of: HTTPBearer
  description: The same credential, under the scheme name used in the older refuel-ai-applications-api-openapi.yml. Not a second mechanism.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/refuel-ai-applications-api-openapi.yml
  type: http
slug: refuel-ai-authentication
source_filename: refuel-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: openapi/refuel-ai-applications-api-openapi.yml, openapi/refuel-ai-cloud-api-openapi.yml\ndocs: https://docs.refuel.ai/sdk/python\nsummary:\n  types:\n  - http\n  api_key_in:\n  - header\n  oauth2_flows: []\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  description: >-\n    A Refuel API key sent as an HTTP Bearer token: `Authorization: Bearer <REFUEL_API_KEY>`.\n    One key per team; it is issued in the Refuel app. Refuel's own catalog documentation\n    shows it in use against the label endpoint, and the Python SDK reads it from the\n    REFUEL_API_KEY environment variable (or an `api_key` init option).\n  sources:\n  - openapi/refuel-ai-cloud-api-openapi.yml\n  - openapi/refuel-ai-applications-api-openapi.yml\n  - https://docs.refuel.ai/sdk/python\n  applied_to: '99 of 108 operations in the Cloud API spec declare a HTTPBearer security requirement'\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description:\
  \ >-\n    The same credential, under the scheme name used in the older\n    refuel-ai-applications-api-openapi.yml. Not a second mechanism.\n  sources:\n  - openapi/refuel-ai-applications-api-openapi.yml\n  alias_of: HTTPBearer\nkey_management:\n  issuance: In the Refuel app (https://app.refuel.ai) per team.\n  rotation: Not documented.\n  expiry: Not documented.\n  scopes: none — the key is all-or-nothing across the team's data.\n  exposure_note: >-\n    The TeamSchema component includes `api_key` and `api_key_sha`, so\n    `GET /team` returns the team's own API key in the response body. Any caller (or agent)\n    with the key can re-read the key. Recorded as a governance fact for anyone delegating\n    Refuel access to an agent — see agentic-access/refuel-ai-agentic-access.yml.\nunauthenticated_behaviour:\n  status: 401\n  body: '{\"message\":\"Unauthorized\"}'\n  scope: >-\n    Every path on cloud-api.refuel.ai except `/` and `/openapi.json` — including\n    `/.well-known/*`, `/docs`-adjacent\
  \ paths and `/mcp`. Probed 2026-08-14.\n  note: No operation in the spec declares a 401 response, despite this being the universal behaviour.\nnot_supported:\n- oauth2\n- openIdConnect\n- mutualTLS\n- apiKey-in-query\n- basic-auth\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/refuel-ai/refs/heads/main/authentication/refuel-ai-authentication.yml
summary_line: http · 2 schemes
tags:
- Artificial Intelligence
- LLM
- Data Labeling
- Data Enrichment
- Autolabel
- Machine-Learning
- Data Quality
- Training Data
- Fine Tuning
- Data Transformation
- Entity Resolution
- Content Moderation
---

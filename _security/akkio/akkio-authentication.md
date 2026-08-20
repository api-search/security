---
api_key_in:
- header
- query
- body
api_specs:
- filename: akkio-public-api-openapi.yaml
  format: yaml
  label: Akkio Public API (Beta)
  slug: akkio-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akkio/refs/heads/main/openapi/_original/akkio-public-api-openapi.yaml
- filename: akkio-datasets-api-openapi.yml
  format: yaml
  label: Akkio Datasets API
  slug: akkio-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akkio/refs/heads/main/openapi/akkio-datasets-api-openapi.yml
- filename: akkio-models-api-openapi.yml
  format: yaml
  label: Akkio Models API
  slug: akkio-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akkio/refs/heads/main/openapi/akkio-models-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Akkio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Akkio secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Akkio
provider_slug: akkio
scheme_count: 3
schemes:
- applies_to: /api/v1 (Akkio Public API, beta)
  declared_in_spec: false
  evidence: '''All routes but those marked "API Specification" require the X-API-Key header to be set to a valid API key.'' — info.description of https://api.akkio.com/api/v1/api.yaml, fetched 2026-08-13.'
  in: header
  name: X-API-Key
  parameter: X-API-Key
  sources:
  - https://docs.akkio.com/akkio-docs/concepts/authentication
  - openapi/_original/akkio-public-api-openapi.yaml
  type: apiKey
- applies_to: legacy /v1 GET (datasets, models)
  declared_in_spec: true
  in: query
  name: apiKeyQuery
  parameter: api_key
  sources:
  - openapi/_original/akkio-api-openapi.yml
  - https://docs.akkio.com/akkio-docs/endpoints-and-schemas/endpoints/datasets
  type: apiKey
- applies_to: legacy /v1 POST and DELETE (datasets, models)
  declared_in_spec: false
  in: body
  name: apiKeyBody
  parameter: api_key
  sources:
  - https://docs.akkio.com/akkio-docs/endpoints-and-schemas/endpoints/models
  - https://github.com/akkio-inc/akkio-python
  type: apiKey
slug: akkio-authentication
source_filename: akkio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://docs.akkio.com/akkio-docs/concepts/authentication\ndocs: https://docs.akkio.com/akkio-docs/concepts/authentication\nsummary:\n  types: [apiKey]\n  api_key_in: [header, query, body]\n  oauth2_flows: []\n  notes: >-\n    Akkio authenticates every request with a single team-scoped API key, issued\n    and rotated from the Team Settings page of the app. There are THREE distinct\n    placements in production, and which one applies depends on which of Akkio's\n    two API generations you are calling. The current /api/v1 public beta API\n    requires the key in an X-API-Key HEADER on every route except the two\n    \"API Specification\" routes (/api/v1/api.yaml and /api/v1/docs), which are\n    anonymous — that rule is stated in the published spec's own info.description.\n    The legacy /v1 datasets/models API instead takes the key as an `api_key`\n    QUERY parameter on GET and as an `api_key` JSON BODY field on POST/DELETE.\n\
  \    There is no OAuth 2.0 or OIDC surface for API consumers, so no scopes/\n    artifact is produced. Neither published OpenAPI document declares a\n    securitySchemes block at all, so a generated client will not wire auth\n    automatically — the requirement exists only in prose and in info.description.\nschemes:\n- name: X-API-Key\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  applies_to: /api/v1 (Akkio Public API, beta)\n  declared_in_spec: false\n  sources:\n  - https://docs.akkio.com/akkio-docs/concepts/authentication\n  - openapi/_original/akkio-public-api-openapi.yaml\n  evidence: >-\n    'All routes but those marked \"API Specification\" require the X-API-Key header\n    to be set to a valid API key.' — info.description of\n    https://api.akkio.com/api/v1/api.yaml, fetched 2026-08-13.\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  applies_to: legacy /v1 GET (datasets, models)\n  declared_in_spec: true\n  sources:\n  - openapi/_original/akkio-api-openapi.yml\n\
  \  - https://docs.akkio.com/akkio-docs/endpoints-and-schemas/endpoints/datasets\n- name: apiKeyBody\n  type: apiKey\n  in: body\n  parameter: api_key\n  applies_to: legacy /v1 POST and DELETE (datasets, models)\n  declared_in_spec: false\n  sources:\n  - https://docs.akkio.com/akkio-docs/endpoints-and-schemas/endpoints/models\n  - https://github.com/akkio-inc/akkio-python\nanonymous_routes:\n- path: /api/v1/api.yaml\n  note: Returns the public OpenAPI 3.1.0 YAML document; verified anonymous 200 on 2026-08-13.\n- path: /api/v1/docs\n  note: Swagger UI for the public API; verified anonymous 200 on 2026-08-13.\n- path: /openapi.json\n  note: >-\n    The full FastAPI application schema is also served anonymously at the API\n    host root; verified 200 on 2026-08-13. Not documented as a public route.\n- path: /version\n  note: Returns the build sha as text/plain; verified anonymous 200 on 2026-08-13.\n- path: /health\n  note: Verified anonymous 200 on 2026-08-13.\nkey_management:\n  issue_url:\
  \ https://app.akkio.com/team-settings\n  scope: team / organization\n  rotation: Self-service from Team Settings; no documented rotation policy or expiry.\n  note: >-\n    Authorization is organization-scoped: a 403 means the organization behind the\n    key lacks access to the resource, per the authentication docs. There are no\n    per-key scopes or permissions to narrow a key.\nfailure_semantics:\n  '401': Missing, incorrect, or whitespace-padded X-API-Key.\n  '403': The key's organization does not have access to the requested resource.\n  note: See errors/akkio-problem-types.yml.\ngaps:\n- Neither published OpenAPI document declares components.securitySchemes.\n- No OAuth 2.0 / OIDC option for API consumers; no per-key scopes.\n- Three different key placements across two API generations, none machine-declared.\ncross_links:\n  conventions: conventions/akkio-conventions.yml\n  errors: errors/akkio-problem-types.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/akkio/refs/heads/main/authentication/akkio-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Company
- Ai Apps
- Machine-Learning
- Predictive Analytics
- No-Code
- Data Science
- Marketing
- Media
- Audience Modeling
- Predictions
---

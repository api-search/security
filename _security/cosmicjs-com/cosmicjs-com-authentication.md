---
anonymous_access: false
api_key_in:
- query
api_specs:
- filename: cosmicjs-com-blocks-api-openapi.yml
  format: yaml
  label: Cosmic Blocks API
  slug: cosmicjs-com-blocks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cosmicjs-com/openapi/cosmicjs-com-blocks-api-openapi.yml
- filename: cosmicjs-com-media-api-openapi.yml
  format: yaml
  label: Cosmic Media API
  slug: cosmicjs-com-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cosmicjs-com/openapi/cosmicjs-com-media-api-openapi.yml
- filename: cosmicjs-com-object-revisions-api-openapi.yml
  format: yaml
  label: Cosmic Object revisions API
  slug: cosmicjs-com-object-revisions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cosmicjs-com/openapi/cosmicjs-com-object-revisions-api-openapi.yml
- filename: cosmicjs-com-object-types-api-openapi.yml
  format: yaml
  label: Cosmic Object types API
  slug: cosmicjs-com-object-types-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cosmicjs-com/openapi/cosmicjs-com-object-types-api-openapi.yml
- filename: cosmicjs-com-objects-api-openapi.yml
  format: yaml
  label: Cosmic Objects API
  slug: cosmicjs-com-objects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cosmicjs-com/openapi/cosmicjs-com-objects-api-openapi.yml
- filename: cosmicjs-com-status-api-openapi.yml
  format: yaml
  label: Cosmic Status API
  slug: cosmicjs-com-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cosmicjs-com/openapi/cosmicjs-com-status-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Cosmic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cosmic secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Cosmic
provider_slug: cosmicjs-com
scheme_count: 2
schemes:
- description: The Bucket read key, passed as a query parameter. Grants read access to a single Bucket and nothing else. Find it under Bucket > Settings > API Access in the dashboard. Buckets with no read key configured accept reads without one.
  in: query
  name: readKey
  parameter: read_key
  sources:
  - openapi/cosmicjs-com-openapi.yml
  type: apiKey
- description: 'The Bucket write key, passed as `Authorization: Bearer <write_key>`. Grants read and write access to a single Bucket and nothing else. Find it under Bucket > Settings > API Access in the dashboard. The bare key without the `Bearer ` prefix is also accepted, but `Bearer` is the documented form. Buckets with no write key configured accept writes without one.'
  name: writeKey
  scheme: bearer
  sources:
  - openapi/cosmicjs-com-openapi.yml
  type: http
slug: cosmicjs-com-authentication
source_filename: cosmicjs-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://www.cosmicjs.com/docs/api/authentication.md\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: readKey\n  type: apiKey\n  in: query\n  parameter: read_key\n  description: The Bucket read key, passed as a query parameter. Grants read access to a single Bucket and nothing\n    else. Find it under Bucket > Settings > API Access in the dashboard. Buckets with no read key configured accept\n    reads without one.\n  sources:\n  - openapi/cosmicjs-com-openapi.yml\n- name: writeKey\n  type: http\n  scheme: bearer\n  description: 'The Bucket write key, passed as `Authorization: Bearer <write_key>`. Grants read and write access\n    to a single Bucket and nothing else. Find it under Bucket > Settings > API Access in the dashboard. The bare\n    key without the `Bearer ` prefix is also accepted, but `Bearer` is the documented form. Buckets with no write\n    key configured accept writes without\
  \ one.'\n  sources:\n  - openapi/cosmicjs-com-openapi.yml\ndocs: https://www.cosmicjs.com/docs/api/authentication\nderived_from: openapi/cosmicjs-com-openapi.yml\ndocumented_credentials:\n- name: Bucket read key\n  use: read access to one Bucket (read_key query parameter)\n  where: Bucket Settings > API Access\n- name: Bucket write key\n  use: 'writes to one Bucket via Authorization: Bearer header'\n  note: Never expose your Bucket write key in any client-side code.\n- name: Personal Access Token\n  prefix: cos_\n  host: dapi.cosmicjs.com\n  use: dashboard-level API access (agents, workflows, account settings); recommended for the Agent messages API\n  note: Tokens use the `cos_` prefix and carry your full account permissions.\n- name: Agent key\n  prefix: agk_\n  use: short-lived bearer token issued by POST /v3/agents/sign-up; authenticates only the agent-flow endpoints (POST\n    /v3/agents/verify, GET /v3/agents/status)\n"
source_yaml_url: https://artifacts.apis.io/cosmicjs-com/authentication/cosmicjs-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Headless CMS
- Content Management
- content-api
- AI Agents
- MCP
- Webhook
- JAMstack
---

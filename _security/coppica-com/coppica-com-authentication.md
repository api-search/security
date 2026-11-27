---
anonymous_access: false
api_key_in: []
api_specs:
- filename: coppica-com-clients-api-openapi.yml
  format: yaml
  label: Coppica Clients API
  slug: coppica-com-clients-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coppica-com/openapi/coppica-com-clients-api-openapi.yml
- filename: coppica-com-deploy-track-api-openapi.yml
  format: yaml
  label: Coppica Deploy & track API
  slug: coppica-com-deploy-track-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coppica-com/openapi/coppica-com-deploy-track-api-openapi.yml
- filename: coppica-com-generation-api-openapi.yml
  format: yaml
  label: Coppica Generation API
  slug: coppica-com-generation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coppica-com/openapi/coppica-com-generation-api-openapi.yml
- filename: coppica-com-learning-loop-api-openapi.yml
  format: yaml
  label: Coppica Learning loop API
  slug: coppica-com-learning-loop-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coppica-com/openapi/coppica-com-learning-loop-api-openapi.yml
- filename: coppica-com-reference-api-openapi.yml
  format: yaml
  label: Coppica Reference API
  slug: coppica-com-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coppica-com/openapi/coppica-com-reference-api-openapi.yml
- filename: coppica-com-resources-api-openapi.yml
  format: yaml
  label: Coppica Resources API
  slug: coppica-com-resources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coppica-com/openapi/coppica-com-resources-api-openapi.yml
- filename: coppica-com-webhooks-api-openapi.yml
  format: yaml
  label: Coppica Webhooks API
  slug: coppica-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coppica-com/openapi/coppica-com-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Coppica Authentication
name_suffix: Authentication
oauth_flows: []
overview: Coppica secures its APIs with http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Coppica
provider_slug: coppica-com
scheme_count: 3
schemes:
- description: 'A Coppica API key, e.g. `Authorization: Bearer cpk_...`. Keys carry read/write/execute scopes.'
  errors:
  - '401 missing_authorization: no Bearer cpk_ header'
  - '401 invalid_api_key: key not found or disabled'
  - '403 missing_scope: key lacks the required scope (read / write / execute)'
  key_management: Keys are created and revoked in the app at Settings -> API Keys; key management isn't available over the API. The cpk_ value is shown once.
  key_prefix: cpk_
  key_scopes:
  - read
  - write
  - execute
  name: bearerAuth
  plan_requirement: API keys come with the Locked In plan and up, and with a trial.
  scheme: bearer
  sources:
  - openapi/coppica-com-openapi.yml
  - https://coppica.com/docs/api
  - https://coppica.com/llms.txt
  type: http
- description: Separate per-client Webhook Key (Bearer ck_...) created on the client's Integrations page, used to POST conversion events server-to-server to https://coppica.com/api/conversions/inbound (not part of the /api/v1 OpenAPI).
  key_prefix: ck_
  name: webhookKey
  scheme: bearer
  sources:
  - https://coppica.com/docs/integrations
  type: http
- description: The hosted MCP server (https://mcp.coppica.com/mcp) takes the same cpk_ API key per request in the Authorization header.
  name: mcpBearer
  scheme: bearer
  sources:
  - https://coppica.com/skills/coppica.mcp.json
  type: http
slug: coppica-com-authentication
source_filename: coppica-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://coppica.com/docs/api\ndocs: https://coppica.com/docs/api\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'A Coppica API key, e.g. `Authorization: Bearer cpk_...`. Keys carry read/write/execute\n    scopes.'\n  key_prefix: cpk_\n  key_scopes:\n  - read\n  - write\n  - execute\n  key_management: Keys are created and revoked in the app at Settings -> API Keys; key management\n    isn't available over the API. The cpk_ value is shown once.\n  plan_requirement: API keys come with the Locked In plan and up, and with a trial.\n  errors:\n  - '401 missing_authorization: no Bearer cpk_ header'\n  - '401 invalid_api_key: key not found or disabled'\n  - '403 missing_scope: key lacks the required scope (read / write / execute)'\n  sources:\n  - openapi/coppica-com-openapi.yml\n  - https://coppica.com/docs/api\n  - https://coppica.com/llms.txt\n- name: webhookKey\n  type:\
  \ http\n  scheme: bearer\n  description: Separate per-client Webhook Key (Bearer ck_...) created on the client's Integrations\n    page, used to POST conversion events server-to-server to https://coppica.com/api/conversions/inbound\n    (not part of the /api/v1 OpenAPI).\n  key_prefix: ck_\n  sources:\n  - https://coppica.com/docs/integrations\n- name: mcpBearer\n  type: http\n  scheme: bearer\n  description: The hosted MCP server (https://mcp.coppica.com/mcp) takes the same cpk_ API key per request\n    in the Authorization header.\n  sources:\n  - https://coppica.com/skills/coppica.mcp.json\nnote: 'Coppica documents no OAuth for its API; key scopes (read, write, execute) are API-key scopes,\n  all three granted by default.'\n"
source_yaml_url: https://artifacts.apis.io/coppica-com/authentication/coppica-com-authentication.yml
summary_line: http · 3 schemes
tags:
- Company
- Marketing
- Copywriting
- Generative AI
- Advertising
- Conversion Tracking
- Attribution
- MCP
- AI Agents
---

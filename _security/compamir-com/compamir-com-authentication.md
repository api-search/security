---
anonymous_access: false
api_key_in: []
api_specs:
- filename: compamir-com-conflicts-api-openapi.yml
  format: yaml
  label: COMPAMIR Conflicts API
  slug: compamir-com-conflicts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compamir-com/openapi/compamir-com-conflicts-api-openapi.yml
- filename: compamir-com-events-api-openapi.yml
  format: yaml
  label: COMPAMIR Events API
  slug: compamir-com-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compamir-com/openapi/compamir-com-events-api-openapi.yml
- filename: compamir-com-keys-api-openapi.yml
  format: yaml
  label: COMPAMIR Keys API
  slug: compamir-com-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compamir-com/openapi/compamir-com-keys-api-openapi.yml
- filename: compamir-com-meta-api-openapi.yml
  format: yaml
  label: COMPAMIR Meta API
  slug: compamir-com-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compamir-com/openapi/compamir-com-meta-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: COMPAMIR Authentication
name_suffix: Authentication
oauth_flows: []
overview: COMPAMIR secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: COMPAMIR
provider_slug: compamir-com
scheme_count: 1
schemes:
- bearerFormat: cmp_live_...
  description: Free REST API key generated on the developer portal with no account or email; the key is shown once. Keys can be rotated or revoked via POST /v1/keys/rotate and POST /v1/keys/revoke, authenticated with the key itself (no quota used).
  header: 'Authorization: Bearer cmp_live_…'
  name: bearerApiKey
  scheme: bearer
  sources:
  - openapi/compamir-com-openapi.yml
  - https://compamir.com/data.html
  type: http
slug: compamir-com-authentication
source_filename: compamir-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://compamir.com/data.html\ndocs: https://compamir.com/data.html\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerApiKey\n  type: http\n  scheme: bearer\n  bearerFormat: cmp_live_...\n  header: 'Authorization: Bearer cmp_live_…'\n  description: Free REST API key generated on the developer portal with no account or email; the key is shown once. Keys can be rotated or revoked via POST /v1/keys/rotate and POST /v1/keys/revoke, authenticated with the key itself (no quota used).\n  sources:\n  - openapi/compamir-com-openapi.yml\n  - https://compamir.com/data.html\nunauthenticated_surfaces:\n- endpoint: https://api.compamir.com/mcp\n  note: 'Docs: \"The MCP endpoint https://api.compamir.com/mcp is free and unauthenticated.\"'\n"
source_yaml_url: https://artifacts.apis.io/compamir-com/authentication/compamir-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- News
- Media Monitoring
- Fact Comparison
- MCP
- AI Agents
- Japanese
- REST API
---

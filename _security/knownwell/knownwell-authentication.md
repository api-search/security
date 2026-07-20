---
api_key_in:
- header
api_specs:
- filename: knownwell-ci-openapi-original.json
  format: json
  label: Knownwell API
  slug: knownwell-ci
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knownwell/refs/heads/main/openapi/knownwell-ci-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Knownwell Authentication
name_suffix: Authentication
oauth_flows: []
overview: Knownwell secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Knownwell
provider_slug: knownwell
scheme_count: 1
schemes:
- description: The Knownwell API uses API key authentication via HTTP headers. Include your API key in the X-API-Key header with every request. Requests without proper authentication return a 401 Unauthorized error.
  docs: https://api.knownwell.com/docs#authentication
  in: header
  name: APIKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/knownwell-ci-openapi-original.json
  type: apiKey
slug: knownwell-authentication
source_filename: knownwell-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/knownwell-ci-openapi-original.json\ndocs: https://api.knownwell.com/docs#authentication\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  read_only: true\nschemes:\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/knownwell-ci-openapi-original.json\n  docs: https://api.knownwell.com/docs#authentication\n  description: 'The Knownwell API uses API key authentication via HTTP headers. Include your\n    API key in the X-API-Key header with every request. Requests without proper authentication\n    return a 401 Unauthorized error.'\nkey_management:\n  issuance: 'Generate an API key from Integrations > API Connector in the Knownwell dashboard\n    (https://ci.knownwell.com/).'\n  scope: read_only\n  scope_note: 'The OpenAPI APIKeyScope enum has a single value, read_only, documented as \"API\n    key access scope - ALL KEYS ARE READ-ONLY\".\
  \ No write, update, or delete operations are\n    permitted with an API key.'\n  key_scoped_to: customer_id\n  expiration: 'Optional. API keys may be created with expires_days; omitting it creates a\n    non-expiring key (openapi APIKeyCreate.expires_days).'\n  management_operations:\n  - create_api_key_v1_api_keys_post\n  - list_api_keys_v1_api_keys_get\n  - revoke_api_key_v1_api_keys__key_id__delete\nbest_practices:\n- Never expose your API key in client-side code or public repositories\n- Store securely in environment variables or secure vaults\n- Rotate regularly — request new keys periodically\n- Use HTTPS only — all API calls must use HTTPS\n- Monitor usage — track API usage for unauthorized access\nexample: |\n  curl https://api.knownwell.com/ci/v1/clients \\\n    -H \"X-API-Key: your_api_key_here\"\nnotes:\n- No OAuth 2.0 or OpenID Connect surface is published; scopes/ is therefore not applicable.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/knownwell/refs/heads/main/authentication/knownwell-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Commercial Intelligence
- Client Intelligence
- Customer Success
- Revenue Operations
- Professional Services
- Artificial Intelligence
- Analytics
- CRM
- Churn Risk
---

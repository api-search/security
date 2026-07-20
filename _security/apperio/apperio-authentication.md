---
api_key_in:
- header
api_specs:
- filename: apperio-openapi-original.yml
  format: yaml
  label: Apperio API
  slug: apperio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apperio/refs/heads/main/openapi/apperio-openapi-original.yml
auth_types:
- apiKey
description: Apperio authenticates every API request with a user-scoped API token supplied in the HTTP Authorization header using the "Token" scheme. The OpenAPI does not declare a securityScheme, so this profile is captured from the published docs.
kind: authentication
layout: security
method: searched
name: Apperio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apperio secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Apperio
provider_slug: apperio
scheme_count: 1
schemes:
- format: 'Authorization: Token <TOKEN VALUE>'
  in: header
  management: Tokens are self-managed via the Users endpoints (GET/POST /api/v1/users/tokens/, DELETE /api/v1/users/tokens/{token-id}/, PUT /api/v1/users/tokens/{token-id}/status/). Apperio cannot recover a lost token; a new one must be generated.
  name: ApiToken
  parameter: Authorization
  provisioning: Create an API Key from the profile page in the Apperio application; contact Customer Success to enable API access on the account.
  scope: A token carries all capabilities of the user who created it (business or law-firm side). Apperio recommends least-privilege service accounts and cycling the key at least every 12 months.
  sources:
  - openapi/apperio-openapi-original.yml
  type: apiKey
slug: apperio-authentication
source_filename: apperio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://developer.apperio.com/ — Authentication section of the Apperio API Documentation\ndocs: https://developer.apperio.com/\ndescription: >-\n  Apperio authenticates every API request with a user-scoped API token supplied\n  in the HTTP Authorization header using the \"Token\" scheme. The OpenAPI does not\n  declare a securityScheme, so this profile is captured from the published docs.\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n  - name: ApiToken\n    type: apiKey\n    in: header\n    parameter: Authorization\n    format: 'Authorization: Token <TOKEN VALUE>'\n    scope: >-\n      A token carries all capabilities of the user who created it (business or\n      law-firm side). Apperio recommends least-privilege service accounts and\n      cycling the key at least every 12 months.\n    provisioning: >-\n      Create an API Key from the profile page in the Apperio application; contact\n\
  \      Customer Success to enable API access on the account.\n    management: >-\n      Tokens are self-managed via the Users endpoints\n      (GET/POST /api/v1/users/tokens/, DELETE /api/v1/users/tokens/{token-id}/,\n      PUT /api/v1/users/tokens/{token-id}/status/). Apperio cannot recover a lost\n      token; a new one must be generated.\n    sources: [openapi/apperio-openapi-original.yml]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apperio/refs/heads/main/authentication/apperio-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Legal
- Legal Spend Management
- Legal Tech
- E-Billing
- Matter Management
- Legal Operations
- Analytics
- Company
---

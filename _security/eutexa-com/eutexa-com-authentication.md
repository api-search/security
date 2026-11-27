---
anonymous_access: false
api_key_in: []
api_specs:
- filename: eutexa-com-openapi-generated.yml
  format: yaml
  label: Eutexa API
  slug: eutexa-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eutexa-com/openapi/_ae-authored/eutexa-com-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Eutexa Authentication
name_suffix: Authentication
oauth_flows: []
overview: Eutexa declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Eutexa
provider_slug: eutexa-com
scheme_count: 2
schemes:
- description: Workspace‑scoped secret sent as a header. Limited to the scopes you choose.
  in: header
  name: X-Api-Key
  type: apiKey
- authorizationUrl: https://api.eutexa.com/api/v1/oauth/authorize
  description: OAuth2 Authorization Code grant for platforms (Zapier app).
  flow: authorizationCode
  scopes: {}
  tokenUrl: https://api.eutexa.com/api/v1/oauth/token
  type: oauth2
slug: eutexa-com-authentication
source_filename: eutexa-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: searched\nsource: \"https://eutexa.com/docs/api\"\nschemes:\n  - type: apiKey\n    name: X-Api-Key\n    in: header\n    description: \"Workspace‑scoped secret sent as a header. Limited to the scopes you choose.\"\n  - type: oauth2\n    flow: authorizationCode\n    authorizationUrl: \"https://api.eutexa.com/api/v1/oauth/authorize\"\n    tokenUrl: \"https://api.eutexa.com/api/v1/oauth/token\"\n    scopes: {}\n    description: \"OAuth2 Authorization Code grant for platforms (Zapier app).\"\n"
source_yaml_url: https://artifacts.apis.io/eutexa-com/authentication/eutexa-com-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- CRM
- Software-as-a-Service
- B2B
- Automation
---

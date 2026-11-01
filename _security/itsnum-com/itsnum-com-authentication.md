---
anonymous_access: false
api_key_in: []
api_specs:
- filename: itsnum-com-agent-api-openapi.yml
  format: yaml
  label: itsnum-com Agent API
  slug: itsnum-com-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/itsnum-com/openapi/itsnum-com-agent-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Itsnum Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: itsnum-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: itsnum-com
provider_slug: itsnum-com
scheme_count: 2
schemes:
- description: Bearer token numa_live_... for Agent API
  scheme: bearer
  type: http
- description: OAuth 2.1 with PKCE for Partner API
  flow: authorizationCode
  pkce: true
  type: oauth2
slug: itsnum-com-authentication
source_filename: itsnum-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: searched\nsource: https://itsnum.com/agents/\nschemes:\n  - type: http\n    scheme: bearer\n    description: \"Bearer token numa_live_... for Agent API\"\n  - type: oauth2\n    flow: authorizationCode\n    pkce: true\n    description: \"OAuth 2.1 with PKCE for Partner API\"\n"
source_yaml_url: https://artifacts.apis.io/itsnum-com/authentication/itsnum-com-authentication.yml
summary_line: 2 schemes
tags:
- Travel
- eSIM
- Telecom
- Marketplace
- API
- Company
---

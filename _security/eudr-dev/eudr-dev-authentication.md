---
anonymous_access: false
api_key_in: []
api_specs:
- filename: eudr-dev-a2a-api-openapi.yml
  format: yaml
  label: eudr.dev A2a API
  slug: eudr-dev-a2a-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eudr-dev/openapi/eudr-dev-a2a-api-openapi.yml
- filename: eudr-dev-agent-api-openapi.yml
  format: yaml
  label: eudr.dev Agent API
  slug: eudr-dev-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eudr-dev/openapi/eudr-dev-agent-api-openapi.yml
- filename: eudr-dev-discovery-api-openapi.yml
  format: yaml
  label: eudr.dev Discovery API
  slug: eudr-dev-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eudr-dev/openapi/eudr-dev-discovery-api-openapi.yml
- filename: eudr-dev-engineer-api-openapi.yml
  format: yaml
  label: eudr.dev Engineer API
  slug: eudr-dev-engineer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eudr-dev/openapi/eudr-dev-engineer-api-openapi.yml
- filename: eudr-dev-ops-api-openapi.yml
  format: yaml
  label: eudr.dev Ops API
  slug: eudr-dev-ops-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eudr-dev/openapi/eudr-dev-ops-api-openapi.yml
- filename: eudr-dev-public-api-openapi.yml
  format: yaml
  label: eudr.dev Public API
  slug: eudr-dev-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eudr-dev/openapi/eudr-dev-public-api-openapi.yml
- filename: eudr-dev-reference-api-openapi.yml
  format: yaml
  label: eudr.dev Reference API
  slug: eudr-dev-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eudr-dev/openapi/eudr-dev-reference-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: eudr.dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: eudr.dev declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: eudr.dev
provider_slug: eudr-dev
scheme_count: 2
schemes:
- description: 'An API key: sign in at /auth, open /app/#/api-keys, create one (shown once).'
  scheme: bearer
  type: http
- flows:
    authorizationCode:
      authorizationUrl: https://eudr.dev/oauth/authorize
      scopes:
        eudr:read: read the organisation's records
        eudr:write: compile and sign statements
      tokenUrl: https://eudr.dev/oauth/token
  type: oauth2
slug: eudr-dev-authentication
source_filename: eudr-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: derived\nsource: https://eudr.dev/openapi.json\nschemes:\n  - type: http\n    scheme: bearer\n    description: \"An API key: sign in at /auth, open /app/#/api-keys, create one (shown once).\"\n  - type: oauth2\n    flows:\n      authorizationCode:\n        authorizationUrl: https://eudr.dev/oauth/authorize\n        tokenUrl: https://eudr.dev/oauth/token\n        scopes:\n          eudr:read: \"read the organisation's records\"\n          eudr:write: \"compile and sign statements\"\n"
source_yaml_url: https://artifacts.apis.io/eudr-dev/authentication/eudr-dev-authentication.yml
summary_line: 2 schemes
tags:
- EU Deforestation
- Compliance
- Agriculture
- Artificial Intelligence
- Environmental
---

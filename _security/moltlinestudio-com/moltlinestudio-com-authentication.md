---
anonymous_access: false
api_key_in: []
api_specs:
- filename: moltlinestudio-com-agent-check-api-openapi.yml
  format: yaml
  label: moltlinestudio-com Agent Check API
  slug: moltlinestudio-com-agent-check-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/moltlinestudio-com/openapi/moltlinestudio-com-agent-check-api-openapi.yml
- filename: moltlinestudio-com-auth-md-api-openapi.yml
  format: yaml
  label: moltlinestudio-com Auth.md API
  slug: moltlinestudio-com-auth-md-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/moltlinestudio-com/openapi/moltlinestudio-com-auth-md-api-openapi.yml
- filename: moltlinestudio-com-badge-api-openapi.yml
  format: yaml
  label: moltlinestudio-com Badge API
  slug: moltlinestudio-com-badge-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/moltlinestudio-com/openapi/moltlinestudio-com-badge-api-openapi.yml
- filename: moltlinestudio-com-premium-api-openapi.yml
  format: yaml
  label: moltlinestudio-com Premium API
  slug: moltlinestudio-com-premium-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/moltlinestudio-com/openapi/moltlinestudio-com-premium-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Moltlinestudio Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: moltlinestudio-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: moltlinestudio-com
provider_slug: moltlinestudio-com
scheme_count: 2
schemes:
- claim_endpoint: https://moltlinestudio.com/
  credential_types_supported:
  - license_key
  description: Anonymous access with optional license key for premium tools.
  registration_endpoint: https://moltlinestudio.com/
  type: anonymous
- description: OAuth 2.0 discovery metadata is published but interactive flows not offered.
  type: oauth2
  well_known:
  - /.well-known/oauth-authorization-server
  - /.well-known/oauth-protected-resource
slug: moltlinestudio-com-authentication
source_filename: moltlinestudio-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: searched\nsource: https://moltlinestudio.com/auth.md\nschemes:\n  - type: anonymous\n    description: Anonymous access with optional license key for premium tools.\n    credential_types_supported:\n      - license_key\n    registration_endpoint: https://moltlinestudio.com/\n    claim_endpoint: https://moltlinestudio.com/\n  - type: oauth2\n    description: OAuth 2.0 discovery metadata is published but interactive flows not offered.\n    well_known:\n      - /.well-known/oauth-authorization-server\n      - /.well-known/oauth-protected-resource\n"
source_yaml_url: https://artifacts.apis.io/moltlinestudio-com/authentication/moltlinestudio-com-authentication.yml
summary_line: 2 schemes
tags:
- AI
- MCP
- Agent Skills
- Platform
- Tools
---

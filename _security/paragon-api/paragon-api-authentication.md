---
api_key_in: []
api_specs:
- filename: paragon-api-openapi.yml
  format: yaml
  label: Paragon Connect API
  slug: paragon-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragon-api/refs/heads/main/openapi/paragon-api-openapi.yml
- filename: paragon-api-openapi.yml
  format: yaml
  label: Paragon Workflows API
  slug: paragon-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragon-api/refs/heads/main/openapi/paragon-api-openapi.yml
- filename: paragon-api-openapi.yml
  format: yaml
  label: Paragon ActionKit API
  slug: paragon-actionkit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragon-api/refs/heads/main/openapi/paragon-api-openapi.yml
- filename: paragon-api-openapi.yml
  format: yaml
  label: Paragon Proxy API
  slug: paragon-proxy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragon-api/refs/heads/main/openapi/paragon-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: researched
name: Paragon Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Paragon secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Paragon
provider_slug: paragon-api
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'Paragon User Token - an RS256-signed JWT that identifies a Connected User - passed as `Authorization: Bearer <token>`. The SaaS builder''s server signs the token with a private Signing Key generated in the Paragon dashboard under Settings > SDK Setup; Paragon verifies the signature with the matching public key. Minimum claims are `sub` (the Connected User''s or their company''s ID), `aud` (audience, formatted as `useparagon.com/{projectId}`), `iat` (issued-at), and `exp` (expiry, typically one hour). Optional JWT Permissions scope claims (e.g. `actionkit`) restrict which APIs a token may call. The same Bearer token authenticates the Connect/SDK API (api.useparagon.com), the Workflows API, the ActionKit API (actionkit.useparagon.com), and the Proxy API (proxy.useparagon.com).'
  name: paragonUserToken
  scheme: bearer
  sources:
  - https://docs.useparagon.com/getting-started/installing-the-connect-sdk
  - https://docs.useparagon.com/apis/api-reference
  - https://docs.useparagon.com/apis/api-reference/jwt-permissions
  type: http
slug: paragon-api-authentication
source_filename: paragon-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: researched\nsource: https://docs.useparagon.com/getting-started/installing-the-connect-sdk\nsummary:\n  types:\n  - http\nschemes:\n- name: paragonUserToken\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: >-\n    Paragon User Token - an RS256-signed JWT that identifies a Connected User -\n    passed as `Authorization: Bearer <token>`. The SaaS builder's server signs the\n    token with a private Signing Key generated in the Paragon dashboard under\n    Settings > SDK Setup; Paragon verifies the signature with the matching public\n    key. Minimum claims are `sub` (the Connected User's or their company's ID),\n    `aud` (audience, formatted as `useparagon.com/{projectId}`), `iat` (issued-at),\n    and `exp` (expiry, typically one hour). Optional JWT Permissions scope claims\n    (e.g. `actionkit`) restrict which APIs a token may call. The same Bearer token\n    authenticates the Connect/SDK API (api.useparagon.com), the Workflows\
  \ API, the\n    ActionKit API (actionkit.useparagon.com), and the Proxy API\n    (proxy.useparagon.com).\n  sources:\n  - https://docs.useparagon.com/getting-started/installing-the-connect-sdk\n  - https://docs.useparagon.com/apis/api-reference\n  - https://docs.useparagon.com/apis/api-reference/jwt-permissions\nnotes: >-\n  Paragon does not issue a static, project-wide API key for calling these APIs;\n  every call is scoped to a Connected User via a short-lived signed JWT. The\n  Signing Key (an RSA key pair) is the long-lived secret and must be kept on the\n  builder's server. This is a B2B, contact-sales product - obtaining a Project ID\n  and Signing Key requires a Paragon account.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paragon-api/refs/heads/main/authentication/paragon-api-authentication.yml
summary_line: http · 1 scheme
tags:
- Embedded iPaaS
- Integrations
- Embedded Integrations
- Native Integrations
- Workflow Automation
- Integration Platform
- API Integration
- SaaS Integrations
- Connectors
---

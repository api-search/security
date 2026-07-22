---
api_key_in: []
api_specs:
- filename: luminary-openapi-original.yml
  format: yaml
  label: Luminary API
  slug: luminary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luminary/refs/heads/main/openapi/luminary-openapi-original.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Luminary Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Luminary secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Luminary
provider_slug: luminary
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://auth.withluminary.com/oauth2/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://auth.withluminary.com/oauth2/token
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://auth.withluminary.com/oauth2/token
  name: oauth2Profiles
  sources:
  - openapi/luminary-openapi-original.yml
  type: oauth2
slug: luminary-authentication
source_filename: luminary-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/luminary-openapi-original.yml\ndocs: https://api.withluminary.com/.well-known/openid-configuration\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  # From the authorization-server discovery docs (well-known/): PKCE S256 is\n  # supported, plus the device_code grant and refresh_token. SDKs default to the\n  # client_credentials flow (CLIENT_ID / CLIENT_SECRET env vars).\n  discovery:\n  - https://api.withluminary.com/.well-known/openid-configuration\n  - https://api.withluminary.com/.well-known/oauth-authorization-server\n  pkce: S256\n  additional_grants:\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:device_code\n  issuer: https://auth.withluminary.com\nschemes:\n- name: oauth2Profiles\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.withluminary.com/oauth2/authorize\n    tokenUrl: https://auth.withluminary.com/oauth2/token\n\
  \    scopes: 0\n  - flow: clientCredentials\n    tokenUrl: https://auth.withluminary.com/oauth2/token\n    scopes: 0\n  sources:\n  - openapi/luminary-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/luminary/refs/heads/main/authentication/luminary-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Estate Planning
- Wealth Management
- Financial Services
- Legal Tech
- Document AI
- Family Office
- OAuth2
---

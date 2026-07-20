---
api_key_in: []
api_specs:
- filename: c1-openapi-original.yml
  format: yaml
  label: ConductorOne API
  slug: conductorone-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/c1/refs/heads/main/openapi/c1-openapi-original.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: C1 Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: C1 secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: C1
provider_slug: c1
scheme_count: 2
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/c1-openapi-original.yml
  type: http
- description: 'This API uses OAuth2 with the Client Credential flow.

    Client Credentials must be sent in the BODY, not the headers.

    For an example of how to implement this, refer to the [c1TokenSource.Token()](https://github.com/ConductorOne/conductorone-sdk-go/blob/3375fe7c0126d17e7ec4e711693dee7b791023aa/token_source.go#L101-L187) function.'
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: /auth/v1/token
  name: oauth
  sources:
  - openapi/c1-openapi-original.yml
  type: oauth2
slug: c1-authentication
source_filename: c1-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/c1-openapi-original.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/c1-openapi-original.yml\n- name: oauth\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /auth/v1/token\n    scopes: 0\n  description: |-\n    This API uses OAuth2 with the Client Credential flow.\n    Client Credentials must be sent in the BODY, not the headers.\n    For an example of how to implement this, refer to the [c1TokenSource.Token()](https://github.com/ConductorOne/conductorone-sdk-go/blob/3375fe7c0126d17e7ec4e711693dee7b791023aa/token_source.go#L101-L187) function.\n  sources:\n  - openapi/c1-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/c1/refs/heads/main/authentication/c1-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Identity
- Access Management
- IAM
- Identity Governance
- Access Control
- Authorization
- AI Agents
- MCP
- Security
---

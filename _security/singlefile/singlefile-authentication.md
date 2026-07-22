---
api_key_in: []
api_specs:
- filename: singlefile-openapi.yml
  format: yaml
  label: SingleFile External API
  slug: singlefile-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/singlefile/refs/heads/main/openapi/singlefile-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Singlefile Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: SingleFile secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: SingleFile
provider_slug: singlefile
scheme_count: 1
schemes:
- description: 'OAuth 2.0 Client Credentials flow. Exchange client_id/client_secret at the token endpoint for a 1-hour bearer token; send it as Authorization: Bearer <token>.'
  flows:
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://api.demo.singlefile.ai/o/token/
  name: OAuth2ClientCredentials
  sources:
  - openapi/singlefile-openapi.yml
  type: oauth2
slug: singlefile-authentication
source_filename: singlefile-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/singlefile-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.demo.singlefile.ai/o/token/\n    scopes: 2\n  description: 'OAuth 2.0 Client Credentials flow. Exchange client_id/client_secret at the token\n    endpoint for a 1-hour bearer token; send it as Authorization: Bearer <token>.'\n  sources:\n  - openapi/singlefile-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/singlefile/refs/heads/main/authentication/singlefile-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Compliance
- Legal
- Entity Management
- Corporate Compliance
- Registered Agent
- Business Filings
- Regulatory
- API
- Webhooks
- OAuth
---

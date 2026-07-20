---
api_key_in: []
api_specs:
- filename: empirical-security-openapi.yml
  format: yaml
  label: Empirical Security API
  slug: empirical-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/empirical-security/refs/heads/main/openapi/empirical-security-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Empirical Security Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Empirical Security secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Empirical Security
provider_slug: empirical-security
scheme_count: 1
schemes:
- description: OAuth 2.0 client credentials flow via FusionAuth. Exchange client ID/secret (HTTP Basic) for a one-hour JWT access token, then send it as a Bearer token.
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://empiricalsecurity.fusionauth.io/oauth2/token
  name: oauth2
  sources:
  - openapi/empirical-security-openapi.yml
  type: oauth2
slug: empirical-security-authentication
source_filename: empirical-security-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/empirical-security-openapi.yml\ndocs: https://docs.empiricalsecurity.com/authentication\nnotes: >-\n  OAuth 2.0 client credentials via FusionAuth. Create an API Client under\n  Settings -> API Clients in https://app.empiricalsecurity.com/, then POST\n  to the FusionAuth token endpoint with HTTP Basic (client_id:client_secret),\n  grant_type=client_credentials and the target-entity scope. The returned JWT\n  (valid one hour) is sent as Authorization: Bearer <JWT> on API requests.\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://empiricalsecurity.fusionauth.io/oauth2/token\n    scopes: 1\n  description: OAuth 2.0 client credentials flow via FusionAuth. Exchange client ID/secret (HTTP\n    Basic) for a one-hour JWT access token, then send it as a Bearer token.\n  sources:\n  - openapi/empirical-security-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/empirical-security/refs/heads/main/authentication/empirical-security-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Security
- Cybersecurity
- Vulnerability Management
- Vulnerability Prioritization
- CVE
- EPSS
- Exploit Prediction
- Threat Intelligence
---

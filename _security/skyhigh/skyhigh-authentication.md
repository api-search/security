---
api_key_in:
- query
api_specs:
- filename: skyhigh-incidents-openapi-original.yml
  format: yaml
  label: Skyhigh Security SSE Incidents API
  slug: skyhigh-security-sse-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skyhigh/refs/heads/main/openapi/skyhigh-incidents-openapi-original.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Skyhigh Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Skyhigh Security secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Skyhigh Security
provider_slug: skyhigh
scheme_count: 3
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/skyhigh-incidents-openapi-original.yml
  type: http
- in: query
  name: internalApiKey
  parameter: accessToken
  sources:
  - openapi/skyhigh-incidents-openapi-original.yml
  type: apiKey
- flows:
  - authorizationUrl: http://com.shn/api/oauth/dialog
    flow: implicit
    scopes: 3
  name: tenantAuth
  sources:
  - openapi/skyhigh-incidents-openapi-original.yml
  type: oauth2
slug: skyhigh-authentication
source_filename: skyhigh-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/skyhigh-incidents-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - query\n  oauth2_flows:\n  - implicit\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/skyhigh-incidents-openapi-original.yml\n- name: internalApiKey\n  type: apiKey\n  in: query\n  parameter: accessToken\n  sources:\n  - openapi/skyhigh-incidents-openapi-original.yml\n- name: tenantAuth\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: http://com.shn/api/oauth/dialog\n    scopes: 3\n  sources:\n  - openapi/skyhigh-incidents-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skyhigh/refs/heads/main/authentication/skyhigh-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Company
- Cybersecurity
- Security Service Edge
- CASB
- Secure Web Gateway
- Data Loss Prevention
- Cloud Security
- Zero Trust
- SASE
---

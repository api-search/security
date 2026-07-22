---
api_key_in: []
api_specs:
- filename: subspace-openapi-original.yml
  format: yaml
  label: Subspace Product API
  slug: subspace-product-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/subspace/refs/heads/main/openapi/subspace-openapi-original.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Subspace Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Subspace secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Subspace
provider_slug: subspace
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 9
    tokenUrl: https://id.subspace.com/oauth/token
  name: accessCode
  sources:
  - openapi/subspace-openapi-original.yml
  type: oauth2
slug: subspace-authentication
source_filename: subspace-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/subspace-openapi-original.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: accessCode\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://id.subspace.com/oauth/token\n    scopes: 9\n  sources:\n  - openapi/subspace-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/subspace/refs/heads/main/authentication/subspace-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Networking
- Real-Time
- WebRTC
- VoIP
- SIP
- CDN
- Gaming
- Latency
- Infrastructure
---

---
api_key_in: []
api_specs:
- filename: lumen-internet-on-demand-api-openapi.yml
  format: yaml
  label: Lumen Internet On-Demand API
  slug: internet-on-demand-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumen-technologies/refs/heads/main/openapi/lumen-internet-on-demand-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Lumen Technologies Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Lumen Technologies secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Lumen Technologies
provider_slug: lumen-technologies
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://api.lumen.com/oauth2/token
  name: oauth2
  sources:
  - openapi/lumen-internet-on-demand-api-openapi.yml
  type: oauth2
slug: lumen-technologies-authentication
source_filename: lumen-technologies-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lumen-internet-on-demand-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.lumen.com/oauth2/token\n    scopes: 2\n  sources:\n  - openapi/lumen-internet-on-demand-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lumen-technologies/refs/heads/main/authentication/lumen-technologies-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Bandwidth
- Edge Cloud
- Fiber
- Infrastructure
- Internet
- Network
- Networking
- Security
- Telecom
---

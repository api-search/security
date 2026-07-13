---
api_key_in: []
api_specs:
- filename: ciena-blue-planet-openapi.yml
  format: yaml
  label: Ciena Blue Planet Open API
  slug: blue-planet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ciena/refs/heads/main/openapi/ciena-blue-planet-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Ciena Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Ciena secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Ciena
provider_slug: ciena
scheme_count: 1
schemes:
- description: OAuth 2.0 authentication for Blue Planet API
  flows:
  - flow: clientCredentials
    scopes: 5
    tokenUrl: https://api.blueplanet.com/oauth/token
  name: oauth2
  sources:
  - openapi/ciena-blue-planet-openapi.yml
  type: oauth2
slug: ciena-authentication
source_filename: ciena-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ciena-blue-planet-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.blueplanet.com/oauth/token\n    scopes: 5\n  description: OAuth 2.0 authentication for Blue Planet API\n  sources:\n  - openapi/ciena-blue-planet-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ciena/refs/heads/main/authentication/ciena-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- MEF
- NETCONF
- Network Automation
- Network Management
- Optical
- RESTCONF
- SDN
- Telecom
- TM Forum
- Fortune 1000
---

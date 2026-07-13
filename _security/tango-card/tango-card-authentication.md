---
api_key_in: []
api_specs:
- filename: llms.txt
  format: yaml
  label: Tango RaaS API
  slug: tango-raas-api
  spec_type: OpenAPI
  url: https://developers.tangocard.com/llms.txt
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Tango Card Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Tango Card secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Tango Card
provider_slug: tango-card
scheme_count: 2
schemes:
- description: HTTP Basic Auth using platform name and API key
  name: basicAuth
  scheme: basic
  sources:
  - openapi/tango-raas-api-openapi.yml
  type: http
- description: OAuth 2.0 client credentials flow for more secure integrations
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://auth.tangocard.com/oauth/token
  name: oAuth2
  sources:
  - openapi/tango-raas-api-openapi.yml
  type: oauth2
slug: tango-card-authentication
source_filename: tango-card-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tango-raas-api-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Auth using platform name and API key\n  sources:\n  - openapi/tango-raas-api-openapi.yml\n- name: oAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.tangocard.com/oauth/token\n    scopes: 0\n  description: OAuth 2.0 client credentials flow for more secure integrations\n  sources:\n  - openapi/tango-raas-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tango-card/refs/heads/main/authentication/tango-card-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Gift Cards
- Rewards
- Incentives
- Digital Rewards
- Prepaid Cards
- Payments
---

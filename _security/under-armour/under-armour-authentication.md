---
api_key_in: []
api_specs:
- filename: mapmyfitness-openapi.yml
  format: yaml
  label: MapMyFitness API
  slug: mapmyfitness-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/under-armour/refs/heads/main/openapi/mapmyfitness-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Under Armour Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Under Armour secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Under Armour
provider_slug: under-armour
scheme_count: 1
schemes:
- description: OAuth 2.0 authentication
  flows:
  - authorizationUrl: https://www.mapmyfitness.com/v7.1/oauth2/authorize/
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://api.ua.com/v7.1/oauth2/access_token/
  name: oauth2
  sources:
  - openapi/mapmyfitness-openapi.yml
  type: oauth2
slug: under-armour-authentication
source_filename: under-armour-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mapmyfitness-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.mapmyfitness.com/v7.1/oauth2/authorize/\n    tokenUrl: https://api.ua.com/v7.1/oauth2/access_token/\n    scopes: 2\n  description: OAuth 2.0 authentication\n  sources:\n  - openapi/mapmyfitness-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/under-armour/refs/heads/main/authentication/under-armour-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Fitness
- Health
- Wearables
- Connected Fitness
- Sports
- Fortune 1000
---

---
api_key_in: []
api_specs:
- filename: medidata-rave-openapi.yml
  format: yaml
  label: Medidata Rave EDC API
  slug: medidata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medidata/refs/heads/main/openapi/medidata-rave-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Medidata Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: medidata secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: medidata
provider_slug: medidata
scheme_count: 2
schemes:
- description: Medidata Rave username and password
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/medidata-rave-openapi.yml
  type: http
- flows:
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://identity.medidata.com/connect/token
  name: OAuth2
  sources:
  - openapi/medidata-rave-openapi.yml
  type: oauth2
slug: medidata-authentication
source_filename: medidata-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/medidata-rave-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: Medidata Rave username and password\n  sources:\n  - openapi/medidata-rave-openapi.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://identity.medidata.com/connect/token\n    scopes: 2\n  sources:\n  - openapi/medidata-rave-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/medidata/refs/heads/main/authentication/medidata-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags: []
---

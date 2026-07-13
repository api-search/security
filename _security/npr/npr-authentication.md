---
api_key_in: []
api_specs:
- filename: npr-station-finder-openapi-original.yml
  format: yaml
  label: NPR Station Finder
  slug: station-finder
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/npr/main/openapi/npr-station-finder-openapi-original.yml
- filename: npr-identity-openapi-original.yml
  format: yaml
  label: NPR Identity
  slug: identity
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/npr/main/openapi/npr-identity-openapi-original.yml
- filename: npr-authorization-openapi-original.yml
  format: yaml
  label: NPR Authorization
  slug: authorization
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/npr/main/openapi/npr-authorization-openapi-original.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Npr Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: NPR secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: NPR
provider_slug: npr
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://authorization.api.npr.org/v2/authorize
    flow: authorizationCode
    scopes: 5
    tokenUrl: https://authorization.api.npr.org/v2/token
  name: oauth2
  sources:
  - openapi/npr-authorization-openapi-original.yml
  - openapi/npr-identity-openapi-original.yml
  - openapi/npr-station-finder-openapi-original.yml
  type: oauth2
slug: npr-authentication
source_filename: npr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/npr-authorization-openapi-original.yml, openapi/npr-identity-openapi-original.yml,\n  openapi/npr-station-finder-openapi-original.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://authorization.api.npr.org/v2/authorize\n    tokenUrl: https://authorization.api.npr.org/v2/token\n    scopes: 5\n  sources:\n  - openapi/npr-authorization-openapi-original.yml\n  - openapi/npr-identity-openapi-original.yml\n  - openapi/npr-station-finder-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/npr/refs/heads/main/authentication/npr-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Media
- News
- Radio
---

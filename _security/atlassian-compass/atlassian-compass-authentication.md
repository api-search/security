---
api_key_in: []
api_specs:
- filename: atlassian-compass-openapi.yml
  format: yaml
  label: Atlassian Compass REST API
  slug: atlassian-compass-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlassian-compass/refs/heads/main/openapi/atlassian-compass-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Atlassian Compass Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Atlassian Compass secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Atlassian Compass
provider_slug: atlassian-compass
scheme_count: 1
schemes:
- description: OAuth 2.0 (3LO) for Atlassian Cloud
  flows:
  - authorizationUrl: https://auth.atlassian.com/authorize
    flow: authorizationCode
    scopes: 4
    tokenUrl: https://auth.atlassian.com/oauth/token
  name: oauth2
  sources:
  - openapi/atlassian-compass-openapi.yml
  type: oauth2
slug: atlassian-compass-authentication
source_filename: atlassian-compass-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/atlassian-compass-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.atlassian.com/authorize\n    tokenUrl: https://auth.atlassian.com/oauth/token\n    scopes: 4\n  description: OAuth 2.0 (3LO) for Atlassian Cloud\n  sources:\n  - openapi/atlassian-compass-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atlassian-compass/refs/heads/main/authentication/atlassian-compass-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Atlassian
- Component Management
- Developer Experience
- Software Catalog
- GraphQL
---

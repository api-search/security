---
api_key_in: []
api_specs:
- filename: swagger.v3.json
  format: json
  label: Confluence Cloud REST API
  slug: confluence-cloud-rest-api
  spec_type: OpenAPI
  url: https://dac-static.atlassian.com/cloud/confluence/swagger.v3.json
- filename: openapi-v2.v3.json
  format: json
  label: Confluence Cloud REST API V2
  slug: confluence-cloud-rest-api-v2
  spec_type: OpenAPI
  url: https://dac-static.atlassian.com/cloud/confluence/openapi-v2.v3.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Atlassian Confluence Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Atlassian Confluence secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Atlassian Confluence
provider_slug: atlassian-confluence
scheme_count: 2
schemes:
- description: 'Basic auth using your Atlassian account email and an API token

    generated at https://id.atlassian.com/manage-profile/security/api-tokens.'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/atlassian-confluence-openapi.yml
  type: http
- description: OAuth 2.0 (3LO) for Atlassian Cloud Connect/Forge apps
  flows:
  - authorizationUrl: https://auth.atlassian.com/authorize
    flow: authorizationCode
    scopes: 7
    tokenUrl: https://auth.atlassian.com/oauth/token
  name: oauth2
  sources:
  - openapi/atlassian-confluence-openapi.yml
  type: oauth2
slug: atlassian-confluence-authentication
source_filename: atlassian-confluence-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/atlassian-confluence-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: |-\n    Basic auth using your Atlassian account email and an API token\n    generated at https://id.atlassian.com/manage-profile/security/api-tokens.\n  sources:\n  - openapi/atlassian-confluence-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.atlassian.com/authorize\n    tokenUrl: https://auth.atlassian.com/oauth/token\n    scopes: 7\n  description: OAuth 2.0 (3LO) for Atlassian Cloud Connect/Forge apps\n  sources:\n  - openapi/atlassian-confluence-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atlassian-confluence/refs/heads/main/authentication/atlassian-confluence-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Atlassian
- Collaboration
- Content Management
- Documentation
- Knowledge Management
- Wiki
---

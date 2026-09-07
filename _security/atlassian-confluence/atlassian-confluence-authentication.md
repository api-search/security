---
anonymous_access: false
api_key_in: []
api_specs:
- filename: atlassian-confluence-rest-v2-openapi.json
  format: json
  label: Confluence Cloud REST API v2
  slug: confluence-cloud-rest-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlassian-confluence/refs/heads/main/openapi/atlassian-confluence-rest-v2-openapi.json
- filename: atlassian-confluence-rest-v1-openapi.json
  format: json
  label: Confluence Cloud REST API v1
  slug: confluence-cloud-rest-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlassian-confluence/refs/heads/main/openapi/atlassian-confluence-rest-v1-openapi.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
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
- description: You can access this resource via basic auth.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/atlassian-confluence-rest-v1-openapi.json
  - openapi/atlassian-confluence-rest-v2-openapi.json
  type: http
- description: This API uses OAuth 2 with the authorizationCode grant flow.
  flows:
  - authorizationUrl: https://auth.atlassian.com/authorize
    flow: authorizationCode
    scopes: 76
    tokenUrl: https://auth.atlassian.com/oauth/token
  name: oAuthDefinitions
  sources:
  - openapi/atlassian-confluence-rest-v1-openapi.json
  - openapi/atlassian-confluence-rest-v2-openapi.json
  type: oauth2
slug: atlassian-confluence-authentication
source_filename: atlassian-confluence-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: derived\nsource: openapi/atlassian-confluence-rest-v1-openapi.json, openapi/atlassian-confluence-rest-v2-openapi.json\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: You can access this resource via basic auth.\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n  - openapi/atlassian-confluence-rest-v2-openapi.json\n- name: oAuthDefinitions\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.atlassian.com/authorize\n    tokenUrl: https://auth.atlassian.com/oauth/token\n    scopes: 76\n  description: This API uses OAuth 2 with the authorizationCode grant flow.\n  sources:\n  - openapi/atlassian-confluence-rest-v1-openapi.json\n  - openapi/atlassian-confluence-rest-v2-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atlassian-confluence/refs/heads/main/authentication/atlassian-confluence-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Atlassian
- Collaboration
- Content Management
- Documentation
- Knowledge-Management
- Wiki
- MCP
- GraphQL
- Agents
- Productivity
---

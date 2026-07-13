---
api_key_in: []
api_specs:
- filename: swagger.v3.json
  format: json
  label: Confluence Cloud REST API v1
  slug: confluence-cloud-rest-api-v1
  spec_type: OpenAPI
  url: https://dac-static.atlassian.com/cloud/confluence/swagger.v3.json
- filename: openapi.yaml
  format: yaml
  label: Confluence Cloud REST API v2
  slug: confluence-cloud-rest-api-v2
  spec_type: OpenAPI
  url: https://developer.atlassian.com/cloud/confluence/rest/v2/api-spec/
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Confluence Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Confluence secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Confluence
provider_slug: confluence
scheme_count: 3
schemes:
- description: Basic authentication using email and API token. Provide your Atlassian account email as the username and an API token as the password.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/confluence-cloud-v2.yml
  type: http
- description: OAuth 2.0 (3LO) for Confluence Cloud apps.
  flows:
  - authorizationUrl: https://auth.atlassian.com/authorize
    flow: authorizationCode
    scopes: 9
    tokenUrl: https://auth.atlassian.com/oauth/token
  name: oAuth2
  sources:
  - openapi/confluence-cloud-v2.yml
  type: oauth2
- description: Personal Access Token or OAuth 2.0 Bearer token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/confluence-cloud-v2.yml
  type: http
slug: confluence-authentication
source_filename: confluence-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/confluence-cloud-v2.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Basic authentication using email and API token. Provide your Atlassian account\n    email as the username and an API token as the password.\n  sources:\n  - openapi/confluence-cloud-v2.yml\n- name: oAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.atlassian.com/authorize\n    tokenUrl: https://auth.atlassian.com/oauth/token\n    scopes: 9\n  description: OAuth 2.0 (3LO) for Confluence Cloud apps.\n  sources:\n  - openapi/confluence-cloud-v2.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Personal Access Token or OAuth 2.0 Bearer token.\n  sources:\n  - openapi/confluence-cloud-v2.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/confluence/refs/heads/main/authentication/confluence-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Collaboration
- Content Management
- Documentation
- Knowledge Base
- Wiki
---

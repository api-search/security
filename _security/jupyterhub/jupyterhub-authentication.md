---
api_key_in:
- header
api_specs:
- filename: jupyterhub-rest-api-openapi.yml
  format: yaml
  label: JupyterHub REST API
  slug: jupyterhub-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupyterhub/refs/heads/main/openapi/jupyterhub-rest-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Jupyterhub Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: JupyterHub secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: JupyterHub
provider_slug: jupyterhub
scheme_count: 2
schemes:
- description: 'Token-based authentication. Use the form: Authorization: token <token>'
  in: header
  name: token
  parameter: Authorization
  sources:
  - openapi/jupyterhub-rest-api-openapi.yml
  type: apiKey
- flows:
  - authorizationUrl: /hub/api/oauth2/authorize
    flow: authorizationCode
    scopes: 9
    tokenUrl: /hub/api/oauth2/token
  name: oauth2
  sources:
  - openapi/jupyterhub-rest-api-openapi.yml
  type: oauth2
slug: jupyterhub-authentication
source_filename: jupyterhub-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/jupyterhub-rest-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: token\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Token-based authentication. Use the form: Authorization: token <token>'\n  sources:\n  - openapi/jupyterhub-rest-api-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /hub/api/oauth2/authorize\n    tokenUrl: /hub/api/oauth2/token\n    scopes: 9\n  sources:\n  - openapi/jupyterhub-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jupyterhub/refs/heads/main/authentication/jupyterhub-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Authentication
- Data Science
- Education
- Hub
- Multi-User
- Notebooks
- OAuth2
- Python
---

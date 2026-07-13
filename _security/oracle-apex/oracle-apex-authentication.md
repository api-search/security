---
api_key_in: []
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Oracle Apex Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Oracle APEX secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Oracle APEX
provider_slug: oracle-apex
scheme_count: 2
schemes:
- description: HTTP Basic authentication using ORDS-enabled database schema credentials
  name: basicAuth
  scheme: basic
  sources:
  - openapi/ords-rest-api-openapi.json
  type: http
- description: OAuth 2.0 authorization using ORDS OAuth client credentials or authorization code flow
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: /ords/{schema}/oauth/token
  - authorizationUrl: /ords/{schema}/oauth/auth
    flow: authorizationCode
    scopes: 0
    tokenUrl: /ords/{schema}/oauth/token
  name: oauth2
  sources:
  - openapi/ords-rest-api-openapi.json
  type: oauth2
slug: oracle-apex-authentication
source_filename: oracle-apex-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ords-rest-api-openapi.json\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication using ORDS-enabled database schema credentials\n  sources:\n  - openapi/ords-rest-api-openapi.json\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /ords/{schema}/oauth/token\n    scopes: 0\n  - flow: authorizationCode\n    authorizationUrl: /ords/{schema}/oauth/auth\n    tokenUrl: /ords/{schema}/oauth/token\n    scopes: 0\n  description: OAuth 2.0 authorization using ORDS OAuth client credentials or authorization\n    code flow\n  sources:\n  - openapi/ords-rest-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oracle-apex/refs/heads/main/authentication/oracle-apex-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- APEX
- Cloud
- Database
- Development Platform
- Enterprise
- Generative AI
- Low-Code
- Oracle
- ORDS
- PL/SQL
- REST API
- Web Applications
- Workflow
---

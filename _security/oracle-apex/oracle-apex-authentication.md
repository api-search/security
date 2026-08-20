---
api_key_in: []
api_specs:
- filename: oracle-apex-autorest-api-openapi.yml
  format: yaml
  label: Oracle APEX AutoREST API
  slug: oracle-apex-autorest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-apex/refs/heads/main/openapi/oracle-apex-autorest-api-openapi.yml
- filename: oracle-apex-handlers-api-openapi.yml
  format: yaml
  label: Oracle APEX Handlers API
  slug: oracle-apex-handlers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-apex/refs/heads/main/openapi/oracle-apex-handlers-api-openapi.yml
- filename: oracle-apex-modules-api-openapi.yml
  format: yaml
  label: Oracle APEX Modules API
  slug: oracle-apex-modules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-apex/refs/heads/main/openapi/oracle-apex-modules-api-openapi.yml
- filename: oracle-apex-oauth-clients-api-openapi.yml
  format: yaml
  label: Oracle APEX OAuth Clients API
  slug: oracle-apex-oauth-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-apex/refs/heads/main/openapi/oracle-apex-oauth-clients-api-openapi.yml
- filename: oracle-apex-overview-api-openapi.yml
  format: yaml
  label: Oracle APEX Overview API
  slug: oracle-apex-overview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-apex/refs/heads/main/openapi/oracle-apex-overview-api-openapi.yml
- filename: oracle-apex-parameters-api-openapi.yml
  format: yaml
  label: Oracle APEX Parameters API
  slug: oracle-apex-parameters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-apex/refs/heads/main/openapi/oracle-apex-parameters-api-openapi.yml
- filename: oracle-apex-privileges-api-openapi.yml
  format: yaml
  label: Oracle APEX Privileges API
  slug: oracle-apex-privileges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-apex/refs/heads/main/openapi/oracle-apex-privileges-api-openapi.yml
- filename: oracle-apex-properties-api-openapi.yml
  format: yaml
  label: Oracle APEX Properties API
  slug: oracle-apex-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-apex/refs/heads/main/openapi/oracle-apex-properties-api-openapi.yml
- filename: oracle-apex-roles-api-openapi.yml
  format: yaml
  label: Oracle APEX Roles API
  slug: oracle-apex-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-apex/refs/heads/main/openapi/oracle-apex-roles-api-openapi.yml
- filename: oracle-apex-templates-api-openapi.yml
  format: yaml
  label: Oracle APEX Templates API
  slug: oracle-apex-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-apex/refs/heads/main/openapi/oracle-apex-templates-api-openapi.yml
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
- Workflows
---

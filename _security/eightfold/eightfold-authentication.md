---
api_key_in:
- header
api_specs:
- filename: llms.txt
  format: yaml
  label: Eightfold API v2
  slug: eightfold-api-v2
  spec_type: OpenAPI
  url: https://apidocs.eightfold.ai/llms.txt
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Eightfold Authentication
name_suffix: Authentication
oauth_flows:
- password
overview: Eightfold secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password flow(s).
provider_name: Eightfold
provider_slug: eightfold
scheme_count: 2
schemes:
- bearer_header: 'Authorization: Bearer <access_token>'
  flow: password
  name: OAuth2Password
  request:
    content_type: application/json
    fields:
    - grantType
    - username
    - password
    grantType_value: password
    method: POST
  response_token_field: data.access_token
  token_endpoint: https://apiv2.eightfold.ai/oauth/v1/authenticate
  token_ttl_seconds: 8640
  token_type: bearer
  type: oauth2
- name: BasicAuthClientCredentials
  regions:
  - header_present: true
    region: US
  - header_present: true
    region: EU
  - header_present: true
    region: CA
  - header_present: true
    region: ME
  - header_present: true
    region: AP
  - header_present: true
    region: WU
  - header_present: true
    region: Gov
  scheme: basic
  type: http
  usage: Basic-auth header carrying the client id:secret pair used to authorize the token request against the regional /oauth/v1/authenticate endpoint. Distinct per region.
slug: eightfold-authentication
source_filename: eightfold-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://apidocs.eightfold.ai/docs/oauth-configuration\ndocs: https://apidocs.eightfold.ai/docs/eightfold-api-authorization-guide\nsummary:\n  types: [oauth2, http]\n  oauth2_flows: [password]\n  api_key_in: [header]\n  notes: >-\n    OAuth 2.0 resource-owner-password-grant. The API-key credentials (email as user_id,\n    generated API key as password) are presented via HTTP Basic auth to the regional\n    token endpoint to mint a bearer access_token, which is then sent on every API call.\n    Per-key READ/WRITE permission scopes gate each endpoint (see scopes artifact).\nschemes:\n- name: OAuth2Password\n  type: oauth2\n  flow: password\n  token_endpoint: https://apiv2.eightfold.ai/oauth/v1/authenticate\n  request:\n    method: POST\n    content_type: application/json\n    fields: [grantType, username, password]\n    grantType_value: password\n  response_token_field: data.access_token\n  token_type: bearer\n  bearer_header:\
  \ 'Authorization: Bearer <access_token>'\n  token_ttl_seconds: 8640\n- name: BasicAuthClientCredentials\n  type: http\n  scheme: basic\n  usage: >-\n    Basic-auth header carrying the client id:secret pair used to authorize the token\n    request against the regional /oauth/v1/authenticate endpoint. Distinct per region.\n  regions:\n  - {region: US, header_present: true}\n  - {region: EU, header_present: true}\n  - {region: CA, header_present: true}\n  - {region: ME, header_present: true}\n  - {region: AP, header_present: true}\n  - {region: WU, header_present: true}\n  - {region: Gov, header_present: true}\nkey_provisioning:\n  console_path: 'Integration > Eightfold API > Authentication > Generate API Key'\n  admin_url: https://app.eightfold.ai/integrations/api_server_config?tab_id=api_server_config\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eightfold/refs/heads/main/authentication/eightfold-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Company
- Talent Intelligence
- Talent Acquisition
- Talent Management
- Recruiting
- Human Resources
- Workforce Planning
- HRIS
- ATS
- Artificial Intelligence
- SCIM
- REST
---

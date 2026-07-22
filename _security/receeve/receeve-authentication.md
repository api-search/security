---
api_key_in:
- header
api_specs:
- filename: receeve-openapi-original.yml
  format: yaml
  label: Receive Client API
  slug: receive-client-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/receeve/refs/heads/main/openapi/receeve-openapi-original.yml
auth_types:
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Receeve Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Receeve secures its APIs with oauth2 and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Receeve
provider_slug: receeve
scheme_count: 2
schemes:
- bearer_header: 'Authorization: Bearer <access_token>'
  flow: clientCredentials
  name: oauth2_client_credentials
  reusable: true
  sources:
  - openapi/receeve-openapi-original.yml
  - https://docs.indebted.co/docs/receive/integration/use-cases/authentication-use-case
  token_endpoint: https://api.receive-demo.com/v1/oauth2/token
  token_operation: getOauth2Token
  token_request_auth: 'HTTP Basic — Authorization: Basic base64(client_id:client_secret), Content-Type: application/x-www-form-urlencoded'
  token_response_fields:
  - access_token
  - expires_in
  - token_type
  token_ttl_seconds: 3600
  token_type: Bearer
  type: oauth2
- description: The Authorization header on all resource operations carries the OAuth2 Bearer access token obtained from getOauth2Token (not a static long-lived key).
  in: header
  name: api_key
  parameter: Authorization
  sources:
  - openapi/receeve-openapi-original.yml
  type: apiKey
slug: receeve-authentication
source_filename: receeve-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/receeve-openapi-original.yml\ndocs: https://docs.indebted.co/docs/receive/integration/use-cases/authentication-use-case\nsummary:\n  types:\n  - oauth2\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\n  notes: >-\n    Authentication is a two-step OAuth2 client-credentials flow. The OpenAPI spec\n    declares a single apiKey security scheme (Authorization header) because the\n    same Authorization header carries the issued Bearer token on every call; the\n    token itself is obtained from the getOauth2Token operation using HTTP Basic\n    credentials.\nschemes:\n- name: oauth2_client_credentials\n  type: oauth2\n  flow: clientCredentials\n  token_operation: getOauth2Token\n  token_endpoint: https://api.receive-demo.com/v1/oauth2/token\n  token_request_auth: >-\n    HTTP Basic — Authorization: Basic base64(client_id:client_secret),\n    Content-Type: application/x-www-form-urlencoded\n\
  \  token_response_fields:\n  - access_token\n  - expires_in\n  - token_type\n  token_ttl_seconds: 3600\n  token_type: Bearer\n  bearer_header: 'Authorization: Bearer <access_token>'\n  reusable: true\n  sources:\n  - openapi/receeve-openapi-original.yml\n  - https://docs.indebted.co/docs/receive/integration/use-cases/authentication-use-case\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: >-\n    The Authorization header on all resource operations carries the OAuth2 Bearer\n    access token obtained from getOauth2Token (not a static long-lived key).\n  sources:\n  - openapi/receeve-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/receeve/refs/heads/main/authentication/receeve-authentication.yml
summary_line: oauth2/apiKey · 2 schemes
tags:
- Company
- Debt Collection
- Receivables Management
- Debt Servicing
- Collections
- Fintech
- Payments
- Webhooks
- Financial Services
- Dunning
---

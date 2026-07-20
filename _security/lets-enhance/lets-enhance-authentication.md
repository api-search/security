---
api_key_in: []
api_specs:
- filename: lets-enhance-claid-openapi.json
  format: json
  label: Claid API
  slug: claid
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lets-enhance/refs/heads/main/openapi/lets-enhance-claid-openapi.json
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Lets Enhance Authentication
name_suffix: Authentication
oauth_flows:
- password
overview: Let's Enhance secures its APIs with oauth2 and http across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password flow(s).
provider_name: Let's Enhance
provider_slug: lets-enhance
scheme_count: 1
schemes:
- description: OAuth 2.0 bearer token (API key) authorization, per RFC 6750. Send requests over HTTPS with the Authorization header set to `Bearer <YOUR_API_KEY>`; no password is required.
  flows:
  - flow: password
    scopes: 4
    tokenUrl: token
  format: Bearer {YOUR_API_KEY}
  header: Authorization
  in: header
  name: OAuth2PasswordBearer
  sources:
  - openapi/lets-enhance-claid-openapi.json
  - https://docs.claid.ai/authentication
  type: oauth2
slug: lets-enhance-authentication
source_filename: lets-enhance-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/lets-enhance-claid-openapi.json\ndocs: https://docs.claid.ai/authentication\nsummary:\n  types:\n  - oauth2\n  - http\n  oauth2_flows:\n  - password\n  primary_style: bearer-api-key\n  notes: >-\n    The Claid API is authenticated with a long-lived API key presented as an HTTP Bearer token:\n    `Authorization: Bearer {YOUR_API_KEY}`. The published OpenAPI models this as an OAuth 2.0\n    security scheme named `OAuth2PasswordBearer` (RFC 6750 bearer token), but the documented\n    developer flow involves no authorization server round trip and no password — the key is minted\n    in the Claid dashboard and used directly. Keys are shown once at creation time and can be\n    copied or downloaded as a text file.\nschemes:\n- name: OAuth2PasswordBearer\n  type: oauth2\n  in: header\n  header: Authorization\n  format: 'Bearer {YOUR_API_KEY}'\n  flows:\n  - flow: password\n    tokenUrl: token\n    scopes: 4\n  description:\
  \ >-\n    OAuth 2.0 bearer token (API key) authorization, per RFC 6750. Send requests over HTTPS with the\n    Authorization header set to `Bearer <YOUR_API_KEY>`; no password is required.\n  sources:\n  - openapi/lets-enhance-claid-openapi.json\n  - https://docs.claid.ai/authentication\nkey_management:\n  create_url: https://claid.ai/account/api\n  dashboard_url: https://claid.ai/account/overview\n  visibility: API keys are visible only once, at creation time, in the Claid dashboard\n  rotation: keys are created, scoped and deleted from the dashboard API keys page\n  guidance: >-\n    Claid recommends creating API keys with the minimum permission scopes necessary for the use case.\npermission_scopes:\n  docs: https://docs.claid.ai/authentication\n  model: >-\n    Each API key can be granted permissions to perform Storage operations, Image editing operations,\n    or both under an Admin permission scope. Scopes are assigned at key creation time or later via\n    API keys -> Edit key in\
  \ the Claid dashboard.\n  artifact: scopes/lets-enhance-scopes.yml\nfailure_modes:\n- status: 401\n  meaning: Authorization is required — missing or invalid API key\n  error_type: auth\n- status: 403\n  meaning: The API key does not have permission scopes for the requested operation\ntransport:\n  https_required: true\n  tls_version: TLSv1.3\nrelated:\n  scopes: scopes/lets-enhance-scopes.yml\n  conventions: conventions/lets-enhance-conventions.yml\n  errors: errors/lets-enhance-error-codes.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lets-enhance/refs/heads/main/authentication/lets-enhance-authentication.yml
summary_line: oauth2/http · 1 scheme
tags:
- Company
- Artificial Intelligence
- Image Processing
- Image Enhancement
- Image Generation
- Computer Vision
- Ecommerce
- Media
- Photography
- Video Generation
---

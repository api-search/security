---
api_key_in: []
api_specs:
- filename: 360learning-core-api.json
  format: json
  label: 360Learning Core API v2
  slug: 360learning-core-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/360learning/refs/heads/main/openapi/360learning-core-api.json
- filename: 360learning-bulk-api.json
  format: json
  label: 360Learning Bulk API v2
  slug: 360learning-bulk-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/360learning/refs/heads/main/openapi/360learning-bulk-api.json
- filename: 360learning-webhook-api.json
  format: json
  label: 360Learning Webhook API v2
  slug: 360learning-webhook-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/360learning/refs/heads/main/openapi/360learning-webhook-api.json
- filename: 360learning-plugin-api.json
  format: json
  label: 360Learning Plugin API v2
  slug: 360learning-plugin-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/360learning/refs/heads/main/openapi/360learning-plugin-api.json
- filename: 360learning-user-authorized-api.json
  format: json
  label: 360Learning User Authorized API v2
  slug: 360learning-user-authorized-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/360learning/refs/heads/main/openapi/360learning-user-authorized-api.json
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: 360Learning Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: 360Learning secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: 360Learning
provider_slug: 360learning
scheme_count: 1
schemes:
- credentials:
    client_id: Unique identifier for the API client (created by a platform admin in the API v2 admin panel).
    client_secret: Confidential key associated with the client ID.
  description: 'API v2 uses the OAuth 2.0 Client Credentials grant for server-to-server authentication. Exchange a client_id + client_secret for a bearer access token, then send it as `Authorization: Bearer <token>`. Access tokens are valid for 1 hour (3600s). By default API calls execute with platform-admin-level access; scope it down with credential-level scopes.'
  flows:
  - flow: clientCredentials
    tokenUrl: https://app.360learning.com/api/v2/oauth2/token
    tokenUrl_us: https://app.us.360learning.com/api/v2/oauth2/token
  grant: client_credentials
  name: oauth2
  required_headers:
  - name: Authorization
    value: Bearer <access_token>
  - name: 360-api-version
    value: v2.0
  scopes_ref: scopes/360learning-scopes.yml
  sources:
  - openapi/360learning-bulk-api.json
  - openapi/360learning-core-api.json
  - openapi/360learning-plugin-api.json
  - openapi/360learning-user-authorized-api.json
  - openapi/360learning-webhook-api.json
  token_endpoint: /api/v2/oauth2/token
  token_ttl_seconds: 3600
  token_type: Bearer
  type: oauth2
slug: 360learning-authentication
source_filename: 360learning-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://360learning.readme.io/docs/authentication\ndocs: https://360learning.readme.io/docs/authentication\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\n  token_expiry_seconds: 3600\nschemes:\n- name: oauth2\n  type: oauth2\n  grant: client_credentials\n  description: >-\n    API v2 uses the OAuth 2.0 Client Credentials grant for server-to-server\n    authentication. Exchange a client_id + client_secret for a bearer access\n    token, then send it as `Authorization: Bearer <token>`. Access tokens are\n    valid for 1 hour (3600s). By default API calls execute with\n    platform-admin-level access; scope it down with credential-level scopes.\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://app.360learning.com/api/v2/oauth2/token\n    tokenUrl_us: https://app.us.360learning.com/api/v2/oauth2/token\n  token_endpoint: /api/v2/oauth2/token\n  token_type: Bearer\n  token_ttl_seconds: 3600\n\
  \  required_headers:\n  - name: Authorization\n    value: Bearer <access_token>\n  - name: 360-api-version\n    value: v2.0\n  credentials:\n    client_id: Unique identifier for the API client (created by a platform admin in the API v2 admin panel).\n    client_secret: Confidential key associated with the client ID.\n  scopes_ref: scopes/360learning-scopes.yml\n  sources:\n  - openapi/360learning-bulk-api.json\n  - openapi/360learning-core-api.json\n  - openapi/360learning-plugin-api.json\n  - openapi/360learning-user-authorized-api.json\n  - openapi/360learning-webhook-api.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/360learning/refs/heads/main/authentication/360learning-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Edtech
- Learning Management System
- E-Learning
- Training
- Collaborative Learning
- HR Tech
- Skills
- API
---

---
api_key_in: []
api_specs:
- filename: pirsch-access-links-api-openapi.yml
  format: yaml
  label: Pirsch Access Links API
  slug: pirsch-access-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pirsch/refs/heads/main/openapi/pirsch-access-links-api-openapi.yml
- filename: pirsch-authentication-api-openapi.yml
  format: yaml
  label: Pirsch Authentication API
  slug: pirsch-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pirsch/refs/heads/main/openapi/pirsch-authentication-api-openapi.yml
- filename: pirsch-clients-api-openapi.yml
  format: yaml
  label: Pirsch Clients API
  slug: pirsch-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pirsch/refs/heads/main/openapi/pirsch-clients-api-openapi.yml
- filename: pirsch-conversion-goals-api-openapi.yml
  format: yaml
  label: Pirsch Conversion Goals API
  slug: pirsch-conversion-goals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pirsch/refs/heads/main/openapi/pirsch-conversion-goals-api-openapi.yml
- filename: pirsch-domains-api-openapi.yml
  format: yaml
  label: Pirsch Domains API
  slug: pirsch-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pirsch/refs/heads/main/openapi/pirsch-domains-api-openapi.yml
- filename: pirsch-email-reports-api-openapi.yml
  format: yaml
  label: Pirsch Email Reports API
  slug: pirsch-email-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pirsch/refs/heads/main/openapi/pirsch-email-reports-api-openapi.yml
- filename: pirsch-funnels-api-openapi.yml
  format: yaml
  label: Pirsch Funnels API
  slug: pirsch-funnels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pirsch/refs/heads/main/openapi/pirsch-funnels-api-openapi.yml
- filename: pirsch-members-api-openapi.yml
  format: yaml
  label: Pirsch Members API
  slug: pirsch-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pirsch/refs/heads/main/openapi/pirsch-members-api-openapi.yml
- filename: pirsch-short-links-api-openapi.yml
  format: yaml
  label: Pirsch Short Links API
  slug: pirsch-short-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pirsch/refs/heads/main/openapi/pirsch-short-links-api-openapi.yml
- filename: pirsch-statistics-api-openapi.yml
  format: yaml
  label: Pirsch Statistics API
  slug: pirsch-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pirsch/refs/heads/main/openapi/pirsch-statistics-api-openapi.yml
- filename: pirsch-tracking-api-openapi.yml
  format: yaml
  label: Pirsch Tracking API
  slug: pirsch-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pirsch/refs/heads/main/openapi/pirsch-tracking-api-openapi.yml
- filename: pirsch-traffic-management-api-openapi.yml
  format: yaml
  label: Pirsch Traffic Management API
  slug: pirsch-traffic-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pirsch/refs/heads/main/openapi/pirsch-traffic-management-api-openapi.yml
- filename: pirsch-user-api-openapi.yml
  format: yaml
  label: Pirsch User API
  slug: pirsch-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pirsch/refs/heads/main/openapi/pirsch-user-api-openapi.yml
- filename: pirsch-views-api-openapi.yml
  format: yaml
  label: Pirsch Views API
  slug: pirsch-views-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pirsch/refs/heads/main/openapi/pirsch-views-api-openapi.yml
- filename: pirsch-webhooks-api-openapi.yml
  format: yaml
  label: Pirsch Webhooks API
  slug: pirsch-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pirsch/refs/heads/main/openapi/pirsch-webhooks-api-openapi.yml
auth_types:
- http
description: Baseline derived mechanically from the OpenAPI securitySchemes, then upgraded from https://docs.pirsch.io/api-sdks/api-guide-v1 and https://docs.pirsch.io/api-sdks/api-v1, which document two distinct credential types the single http/bearer scheme in the spec does not distinguish.
kind: authentication
layout: security
method: searched
name: Pirsch Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pirsch secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Pirsch
provider_slug: pirsch
scheme_count: 1
schemes:
- description: Pass an OAuth2 access token obtained from POST /token, or a static access key, as a Bearer token in the Authorization header.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/pirsch-pirsch-api-openapi.yml
  type: http
slug: pirsch-authentication
source_filename: pirsch-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/_original/pirsch-pirsch-api-openapi.yml\ndocs: https://docs.pirsch.io/api-sdks/api-guide-v1\ndescription: >-\n  Baseline derived mechanically from the OpenAPI securitySchemes, then upgraded\n  from https://docs.pirsch.io/api-sdks/api-guide-v1 and\n  https://docs.pirsch.io/api-sdks/api-v1, which document two distinct credential\n  types the single http/bearer scheme in the spec does not distinguish.\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  credential_types:\n  - oauth2-client-credentials\n  - static-access-key\n  oauth2_flows: []\n  scopes: none\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Pass an OAuth2 access token obtained from POST /token, or a static access key,\n    as a Bearer token in the Authorization header.\n  sources:\n  - openapi/pirsch-pirsch-api-openapi.yml\n\ncredentials:\n- id: oauth-client\n  name: OAuth2 client credentials\n  client_type: oauth\n\
  \  created_via: POST /api/v1/client with type \"oauth\" (operationId createClient), or the dashboard\n  token_endpoint: https://api.pirsch.io/api/v1/token\n  token_request: '{\"client_id\": \"<client_id>\", \"client_secret\": \"<client_secret>\"}'\n  token_response: '{\"access_token\": \"<token>\", \"expires_at\": \"<UTC timestamp>\"}'\n  header: 'Authorization: Bearer <access_token>'\n  access: read and write, scoped to the domain the client belongs to\n  refresh: >-\n    No refresh token. On HTTP 401 the client re-POSTs /token with the same\n    credentials and retries.\n  operation: openapi/pirsch-authentication-api-openapi.yml#getToken\n  docs: https://docs.pirsch.io/api-sdks/api-guide-v1\n- id: access-key\n  name: Access key\n  client_type: token\n  prefix: pa_\n  created_via: POST /api/v1/client with type \"token\" (operationId createClient), or the dashboard\n  header: 'Authorization: Bearer pa_<key>'\n  access: write-only — data submission endpoints only (/hit, /event, /session\
  \ and their batch forms)\n  rotation: >-\n    Delete and recreate the client (DELETE /api/v1/client?id=). No rotation\n    endpoint and no key expiry.\n  purpose: Stateless server-side tracking without a token exchange round trip.\n  docs: https://docs.pirsch.io/api-sdks/api-guide-v1\n\nscopes:\n  supported: false\n  note: >-\n    Pirsch has no OAuth scope surface. A client is either an OAuth client (full\n    read/write on its domain) or a write-only access key; there is nothing\n    finer. No scopes/ artifact is emitted, because an empty scope file would\n    imply a permission model that does not exist.\n\nsecret_exposure:\n  client_secret_returned_once: true\n  detail: >-\n    The Client schema notes client_secret is \"Only returned on creation\" — it\n    cannot be re-read afterwards.\n\ndiscovery:\n  oauth_authorization_server_metadata: false\n  openid_configuration: false\n  note: >-\n    /.well-known/oauth-authorization-server and\n    /.well-known/openid-configuration both returned\
  \ 404 on api.pirsch.io on\n    2026-08-13. There is no machine-discoverable auth metadata; the token\n    endpoint is only findable in the prose docs.\n\ntransport:\n  https_required: true\n  detail: security/pirsch-domain-security.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pirsch/refs/heads/main/authentication/pirsch-authentication.yml
summary_line: http · 1 scheme
tags:
- Analytics
- Web Analytics
- Privacy
- GDPR
- Cookie-Free
- Page Views
- Sessions
- Events
- Conversion Goals
- Funnels
- Traffic Sources
---

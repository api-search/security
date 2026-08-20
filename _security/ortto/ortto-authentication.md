---
api_key_in:
- header
api_specs:
- filename: ortto-accounts-api-openapi.yml
  format: yaml
  label: Ortto Accounts API
  slug: ortto-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ortto/refs/heads/main/openapi/ortto-accounts-api-openapi.yml
- filename: ortto-activities-api-openapi.yml
  format: yaml
  label: Ortto Activities API
  slug: ortto-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ortto/refs/heads/main/openapi/ortto-activities-api-openapi.yml
- filename: ortto-campaigns-api-openapi.yml
  format: yaml
  label: Ortto Campaigns API
  slug: ortto-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ortto/refs/heads/main/openapi/ortto-campaigns-api-openapi.yml
- filename: ortto-people-api-openapi.yml
  format: yaml
  label: Ortto People API
  slug: ortto-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ortto/refs/heads/main/openapi/ortto-people-api-openapi.yml
- filename: ortto-tags-api-openapi.yml
  format: yaml
  label: Ortto Tags API
  slug: ortto-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ortto/refs/heads/main/openapi/ortto-tags-api-openapi.yml
- filename: ortto-transactional-api-openapi.yml
  format: yaml
  label: Ortto Transactional API
  slug: ortto-transactional-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ortto/refs/heads/main/openapi/ortto-transactional-api-openapi.yml
auth_types:
- apiKey
description: 'Ortto authenticates every REST call with a single custom API key sent in the X-Api-Key header. The key is created inside the app (Custom API (advanced) > Get started), is unique to one Ortto account, and carries no user identity — the documentation states keys "do not require or involve any user authentication" and must be treated as a private key. There are no scopes, no per-key permissions, no key prefix and no test-vs-live separation. The one piece of per-key configuration is behavioural rather than authorizational: a default and fallback merge_by field association that determines how person records are matched on write. The MCP server is authenticated separately, with a scoped JWT passed as a query parameter, and is documented in mcp/ortto-mcp.yml.'
kind: authentication
layout: security
method: searched
name: Ortto Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ortto secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Ortto
provider_slug: ortto
scheme_count: 2
schemes:
- description: Custom private API key created in the Ortto app, unique to a single Ortto account, supplied on every request in the X-Api-Key header.
  in: header
  name: ApiKeyAuth
  parameter: X-Api-Key
  per_key_config:
  - description: Default and fallback field association used to match existing person records; overridable per request on merge calls.
    name: merge_by
    source: https://help.ortto.com/a-299-data-source-merge-strategies
  prefix: null
  rotation: Keys can be disconnected at any time through the Ortto user interface; no programmatic rotation endpoint is documented.
  sources:
  - https://help.ortto.com/a-107-configuring-a-custom-api-key
  - openapi/ortto-accounts-api-openapi.yml
  - openapi/ortto-activities-api-openapi.yml
  - openapi/ortto-campaigns-api-openapi.yml
  - openapi/ortto-people-api-openapi.yml
  - openapi/ortto-tags-api-openapi.yml
  - openapi/ortto-transactional-api-openapi.yml
  type: apiKey
- description: Scoped JWT minted in the Ortto app under CDP > Data sources > MCP data source and appended to the MCP endpoint URL. Applies only to the MCP server, not to the REST API.
  in: query
  name: MCPScopedKey
  parameter: jwt
  sources:
  - https://help.ortto.com/a-910-ortto-mcp
  - mcp/ortto-mcp.yml
  surface: mcp
  type: apiKey
slug: ortto-authentication
source_filename: ortto-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  https://help.ortto.com/a-107-configuring-a-custom-api-key,\n  https://help.ortto.com/a-223-developer-guide, upgraded from the securitySchemes\n  in openapi/*.yml\ndocs: https://help.ortto.com/a-107-configuring-a-custom-api-key\ndescription: >-\n  Ortto authenticates every REST call with a single custom API key sent in the\n  X-Api-Key header. The key is created inside the app (Custom API (advanced) >\n  Get started), is unique to one Ortto account, and carries no user identity —\n  the documentation states keys \"do not require or involve any user\n  authentication\" and must be treated as a private key. There are no scopes, no\n  per-key permissions, no key prefix and no test-vs-live separation. The one\n  piece of per-key configuration is behavioural rather than authorizational: a\n  default and fallback merge_by field association that determines how person\n  records are matched on write. The MCP server is authenticated\
  \ separately, with\n  a scoped JWT passed as a query parameter, and is documented in\n  mcp/ortto-mcp.yml.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  scopes: false\n  test_mode_keys: false\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: >-\n    Custom private API key created in the Ortto app, unique to a single Ortto\n    account, supplied on every request in the X-Api-Key header.\n  prefix: null\n  rotation: >-\n    Keys can be disconnected at any time through the Ortto user interface; no\n    programmatic rotation endpoint is documented.\n  per_key_config:\n  - name: merge_by\n    description: >-\n      Default and fallback field association used to match existing person\n      records; overridable per request on merge calls.\n    source: https://help.ortto.com/a-299-data-source-merge-strategies\n  sources:\n  - https://help.ortto.com/a-107-configuring-a-custom-api-key\n\
  \  - openapi/ortto-accounts-api-openapi.yml\n  - openapi/ortto-activities-api-openapi.yml\n  - openapi/ortto-campaigns-api-openapi.yml\n  - openapi/ortto-people-api-openapi.yml\n  - openapi/ortto-tags-api-openapi.yml\n  - openapi/ortto-transactional-api-openapi.yml\n- name: MCPScopedKey\n  type: apiKey\n  in: query\n  parameter: jwt\n  surface: mcp\n  description: >-\n    Scoped JWT minted in the Ortto app under CDP > Data sources > MCP data\n    source and appended to the MCP endpoint URL. Applies only to the MCP server,\n    not to the REST API.\n  sources:\n  - https://help.ortto.com/a-910-ortto-mcp\n  - mcp/ortto-mcp.yml\nfailure_modes:\n- status: 401\n  meaning: Authentication failed or the user does not have permissions.\n- status: 403\n  meaning: Authenticated but not authorized for the resource.\n- note: >-\n    15 failed-credential requests within 15 seconds triggers a 15-second IP ban.\n    See rate-limits/ortto-rate-limits.yml.\napp_login:\n  sso: true\n  okta: true\n  two_factor:\
  \ true\n  note: >-\n    SSO, Okta and 2FA secure human login to the Ortto app; they do not apply to\n    API authentication.\n  source: https://ortto.com/security-privacy/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ortto/refs/heads/main/authentication/ortto-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Marketing Automation
- CDP
- Customer Data Platform
- Analytics
- Email
- SMS
- Transactional Email
- Webhook
- MCP
- Push Notifications
---

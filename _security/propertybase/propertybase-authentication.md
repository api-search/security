---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Propertybase Authentication
name_suffix: Authentication
oauth_flows: []
overview: propertybase declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: propertybase
provider_slug: propertybase
scheme_count: 1
schemes:
- description: Static API key issued by Propertybase support (help@propertybase.com). Sent on every request as the X-BL-API-Key header alongside the account-specific API domain. Anyone holding the key can create, update, and delete records, so it must be kept secret; a compromised key is revoked and reissued by support.
  id: api-key-header
  in: header
  name: X-BL-API-Key
  permissions_model: Each key is granted granular Read / Write / Delete permissions per resource. Requests exceeding a key's permission return an "unauthorized" envelope with a 401 status and an "API Key does not have permissions" error.
  type: apiKey
slug: propertybase-authentication
source_filename: propertybase-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://apidocs.propertybase.com/ (Propertybase GO API authentication section)\ndocs: https://apidocs.propertybase.com/\napi: Propertybase GO API\nsummary: >-\n  The Propertybase GO API authenticates every request with a static, per-account\n  API key passed in a custom HTTP header. Keys are issued by Propertybase support\n  and are all-scope (a single key can read, create, update, and delete records\n  subject to per-resource Read/Write/Delete permissions configured on the key).\n  There is no OAuth 2.0, OpenID Connect, or token-refresh flow documented for this API.\nschemes:\n- id: api-key-header\n  type: apiKey\n  in: header\n  name: X-BL-API-Key\n  description: >-\n    Static API key issued by Propertybase support (help@propertybase.com). Sent on\n    every request as the X-BL-API-Key header alongside the account-specific API\n    domain. Anyone holding the key can create, update, and delete records, so it\n    must be\
  \ kept secret; a compromised key is revoked and reissued by support.\n  permissions_model: >-\n    Each key is granted granular Read / Write / Delete permissions per resource.\n    Requests exceeding a key's permission return an \"unauthorized\" envelope with a\n    401 status and an \"API Key does not have permissions\" error.\ntransport:\n  tls_required: true\n  content_type: application/json\nnotes:\n- Base URL is per-tenant; the account's API domain is provided by Propertybase support.\n- No OAuth2/OIDC scopes, so no scopes/ artifact is derived for this provider.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/propertybase/refs/heads/main/authentication/propertybase-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Real-Estate
- CRM
- PropTech
- Salesforce
- Lead Management
---

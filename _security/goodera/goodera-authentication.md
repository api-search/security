---
api_key_in: []
auth_types: []
description: Authentication profile for Goodera's two published API surfaces. Derived from the provider's own API reference and from a live protocol handshake against the MCP endpoint. No OpenAPI securitySchemes block exists to derive from, because Goodera publishes no OpenAPI document.
kind: authentication
layout: security
method: searched
name: Goodera Authentication
name_suffix: Authentication
oauth_flows: []
overview: Goodera declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Goodera
provider_slug: goodera
scheme_count: 0
schemes: []
slug: goodera-authentication
source_filename: goodera-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: searched\nsource: https://www.goodera.com/resources/api\ndocs: https://www.goodera.com/resources/api\ndescription: >-\n  Authentication profile for Goodera's two published API surfaces. Derived from the\n  provider's own API reference and from a live protocol handshake against the MCP\n  endpoint. No OpenAPI securitySchemes block exists to derive from, because Goodera\n  publishes no OpenAPI document.\nsurfaces:\n- surface: Goodera Developer API\n  base_url: https://developer-api.goodera.com\n  schemes:\n  - id: api-key-header\n    type: apiKey\n    in: header\n    name: x-api-key\n    description: >-\n      Single static API key sent on every authenticated request. Documented verbatim in\n      the reference as: curl --location --request GET\n      'https://developer-api.goodera.com/opportunities/{id}' --header 'x-api-key:\n      <YOUR-API-KEY>'.\n    rotation_documented: false\n    expiry_documented: false\n    scopes: none\n    key_prefix_documented:\
  \ false\n  unauthenticated_surface:\n  - path: /master-data/timezone\n    note: Documented as not requiring the API key.\n  - path: /master-data/country\n    note: Documented as not requiring the API key.\n  - path: /master-data/language\n    note: Documented as not requiring the API key.\n  key_acquisition:\n    self_service: false\n    mechanism: sales-gated request form\n    detail: >-\n      The API reference page carries a \"Request access\" form asking only for a company\n      email address, and confirms \"Our team will follow up within 24 hours!\". There is no\n      developer signup, no self-service key issuance, and no console where a key can be\n      generated or rotated.\n    url: https://www.goodera.com/resources/api\n- surface: Goodera MCP Server\n  base_url: https://mcp.goodera.com/mcp\n  schemes:\n  - id: none\n    type: none\n    description: >-\n      No authentication is enforced at the MCP protocol layer for discovery. initialize and\n      tools/list both returned\
  \ HTTP 200 with no credential supplied and no OAuth challenge.\n    verified: probed\n  oauth_discovery:\n    oauth_protected_resource: 404\n    oauth_authorization_server: 404\n    note: >-\n      RFC 9728 protected-resource metadata is not served, so an MCP client has no way to\n      discover an authorization server for this endpoint.\n  caveat: >-\n    Anonymous discovery is established by probe. API Evangelist did not invoke any tool, so\n    whether tool EXECUTION is also anonymous is not established here.\nobservations:\n- id: no-oauth-anywhere\n  note: >-\n    Neither surface offers OAuth 2.0, OpenID Connect, or scoped delegation. There is no\n    per-user consent model and no way for an end volunteer to authorize a third party\n    against their own data; a partner holds one tenant-wide key.\n- id: no-scope-surface\n  note: >-\n    Because the only credential is a single static header key, there is no scopes artifact\n    to write. Permissions are all-or-nothing at the key level.\n\
  - id: no-mtls-or-signing\n  note: No mutual TLS, request signing, or webhook signature scheme is documented.\n- id: transport-security\n  note: >-\n    Both hosts negotiate TLSv1.3. HSTS is present on www.goodera.com (max-age 31536000) but\n    absent on developer-api.goodera.com and mcp.goodera.com. See\n    security/goodera-domain-security.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/goodera/refs/heads/main/authentication/goodera-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Corporate Volunteering
- Social Impact
- CSR
- Employee Engagement
- Nonprofits
- Events
- Volunteering
- ESG
- Model Context Protocol
---

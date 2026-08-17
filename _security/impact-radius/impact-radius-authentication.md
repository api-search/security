---
api_key_in:
- header
api_specs:
- filename: impact-radius-brand-account-v14.yml
  format: yaml
  label: impact.com Brand API
  slug: impactcom-brand-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/impact-radius/refs/heads/main/openapi/impact-radius-brand-account-v14.yml
- filename: impact-radius-partner-account-v15.yml
  format: yaml
  label: impact.com Partner API
  slug: impactcom-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/impact-radius/refs/heads/main/openapi/impact-radius-partner-account-v15.yml
- filename: impact-radius-agency-advertisers-v3.yml
  format: yaml
  label: impact.com Agency API
  slug: impactcom-agency-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/impact-radius/refs/heads/main/openapi/impact-radius-agency-advertisers-v3.yml
- filename: impact-radius-brand-advocate-account-v13.yml
  format: yaml
  label: impact.com Advocate API
  slug: impactcom-advocate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/impact-radius/refs/heads/main/openapi/impact-radius-brand-advocate-account-v13.yml
auth_types:
- http
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Impact Radius Authentication
name_suffix: Authentication
oauth_flows:
- authorization_code_pkce
overview: Impact Radius secures its APIs with http and apiKey across 6 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorization_code_pkce flow(s).
provider_name: Impact Radius
provider_slug: impact-radius
scheme_count: 6
schemes:
- applies_to:
  - Brand v11-v14
  - Partner v14-v15
  - Agency v2-v3
  - Advocate v1
  declared_in_spec: true
  description: Account SID as username, Auth Token as password, base64-encoded in the Authorization header. The dominant scheme — declared in 27 of the harvested OpenAPI documents and applied globally in the rest.
  name: basicAuth
  scheme: basic
  sources:
  - docs
  - openapi
  spec_count: 27
  type: http
- applies_to:
  - Advocate v1
  declared_in_spec: true
  description: The Advocate specs name the same Basic mechanism `APIKey`. Test-mode and live-mode keys are issued per tenant; the key must match the tenant_alias in the path or the API returns RS003, RS006 or RS032.
  name: APIKey
  scheme: basic
  sources:
  - openapi
  - docs
  spec_count: 9
  type: http
- applies_to:
  - Advocate v1 open/client-facing endpoints
  declared_in_spec: true
  description: Signed per-user JWT for client-side calls made from a browser or mobile app, so a participant can read their own data without the tenant secret being shipped to the client. The Account SID must be carried as a child in the JWT header. Required when Secure Mode is enabled; failures surface as RS005 (checksum required), RS006/RS032 (bad checksum or JWT) and RS045 (missing credentials).
  header_name: X-SaaSquatch-User-Token
  in: header
  name: UserJWT
  sources:
  - openapi
  - docs
  spec_count: 6
  type: apiKey
- applies_to:
  - Brand
  - Partner
  - Agency
  declared_in_spec: false
  description: Fine-grained access tokens created in the account UI (Settings -> Technical -> API -> Create Access Token). Each token pins an API version and toggles API categories with per-category read/write scopes. Presented over the same HTTP Basic Account SID + Auth Token pair, so the wire format is unchanged — the difference is authorization, not authentication. A disabled scoped token, or a call to an endpoint the token does not enable, returns 403 rather than 401.
  in: header
  name: scopedTokens
  sources:
  - docs
  type: apiKey
- applies_to:
  - mcp.impact.com
  declared_in_spec: false
  description: OAuth 2.1 for the hosted MCP server. Per-client MCP usage tokens with refresh tokens; the end user's platform credentials are never shared with the AI assistant, only a revocable token. An administrator can disable MCP account-wide, which deletes existing tokens.
  discovery:
    checked: '2026-08-13'
    note: No RFC 8414 / RFC 9728 / OIDC discovery document is served on any impact.com host.
    oauth_authorization_server: 404
    oauth_protected_resource: 404
    openid_configuration: 404
  name: oauth2.1
  sources:
  - docs
  - probe
  type: oauth2
- applies_to:
  - multi-customer applications
  declared_in_spec: false
  description: impact.com's "Building with LLMs" guide states that multi-customer apps follow OAuth 2.0 Authorization Code + PKCE with documented token rotation. No OAuth endpoints, scopes or registration flow were located on the public developer portal in this pass, and no oauth2 securityScheme appears in any of the 67 published specs — so this is recorded as documented but not machine-readable.
  name: oauth2-authorization-code-pkce
  sources:
  - docs
  type: oauth2
slug: impact-radius-authentication
source_filename: impact-radius-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://integrations.impact.com/brand-api-reference/brand-api-reference-v13/readme/authentication.md\ndocs:\n- https://integrations.impact.com/brand-api-reference/brand-api-reference-v13/readme/authentication.md\n- https://integrations.impact.com/rest-apis/api-quick-start/create-an-api-key.md\n- https://integrations.impact.com/ai-solutions/building-with-llms.md\nderived_from: openapi/ (securitySchemes across 67 documents)\nsummary:\n  types: [http, apiKey]\n  http_scheme: basic\n  api_key_in: [header]\n  oauth2_flows: [authorization_code_pkce]\n  transport: HTTPS only, port 443; plain HTTP fails.\n  failure_status: 401\n  notes: >-\n    The published REST contracts authenticate with HTTP Basic: Account SID is the username (a\n    public identifier, similar to a public API key) and Auth Token is the password (the secret),\n    base64-encoded into `Authorization: Basic base64(AccountSID:AuthToken)`. Scoped Tokens add\n    per-API-category\
  \ read/write least privilege; tokens minted before April 2025 are \"legacy\" and\n    support only read/write or read-only. Advocate additionally accepts a per-participant JWT for\n    client-side calls. OAuth is used off the REST contract: OAuth 2.1 for the hosted MCP server,\n    and — per impact.com's own LLM-integration guidance — OAuth 2.0 Authorization Code + PKCE for\n    multi-customer applications.\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  applies_to: [Brand v11-v14, Partner v14-v15, Agency v2-v3, Advocate v1]\n  declared_in_spec: true\n  spec_count: 27\n  description: >-\n    Account SID as username, Auth Token as password, base64-encoded in the Authorization header.\n    The dominant scheme — declared in 27 of the harvested OpenAPI documents and applied globally\n    in the rest.\n  sources: [docs, openapi]\n- name: APIKey\n  type: http\n  scheme: basic\n  applies_to: [Advocate v1]\n  declared_in_spec: true\n  spec_count: 9\n  description: >-\n    The Advocate\
  \ specs name the same Basic mechanism `APIKey`. Test-mode and live-mode keys are\n    issued per tenant; the key must match the tenant_alias in the path or the API returns RS003,\n    RS006 or RS032.\n  sources: [openapi, docs]\n- name: UserJWT\n  type: apiKey\n  in: header\n  header_name: X-SaaSquatch-User-Token\n  applies_to: [Advocate v1 open/client-facing endpoints]\n  declared_in_spec: true\n  spec_count: 6\n  description: >-\n    Signed per-user JWT for client-side calls made from a browser or mobile app, so a participant\n    can read their own data without the tenant secret being shipped to the client. The Account SID\n    must be carried as a child in the JWT header. Required when Secure Mode is enabled; failures\n    surface as RS005 (checksum required), RS006/RS032 (bad checksum or JWT) and RS045 (missing\n    credentials).\n  sources: [openapi, docs]\n- name: scopedTokens\n  type: apiKey\n  in: header\n  applies_to: [Brand, Partner, Agency]\n  declared_in_spec: false\n  description:\
  \ >-\n    Fine-grained access tokens created in the account UI (Settings -> Technical -> API -> Create\n    Access Token). Each token pins an API version and toggles API categories with per-category\n    read/write scopes. Presented over the same HTTP Basic Account SID + Auth Token pair, so the\n    wire format is unchanged — the difference is authorization, not authentication. A disabled\n    scoped token, or a call to an endpoint the token does not enable, returns 403 rather than 401.\n  sources: [docs]\n- name: oauth2.1\n  type: oauth2\n  applies_to: [mcp.impact.com]\n  declared_in_spec: false\n  description: >-\n    OAuth 2.1 for the hosted MCP server. Per-client MCP usage tokens with refresh tokens; the\n    end user's platform credentials are never shared with the AI assistant, only a revocable\n    token. An administrator can disable MCP account-wide, which deletes existing tokens.\n  discovery:\n    oauth_authorization_server: 404\n    oauth_protected_resource: 404\n    openid_configuration:\
  \ 404\n    checked: '2026-08-13'\n    note: No RFC 8414 / RFC 9728 / OIDC discovery document is served on any impact.com host.\n  sources: [docs, probe]\n- name: oauth2-authorization-code-pkce\n  type: oauth2\n  applies_to: [multi-customer applications]\n  declared_in_spec: false\n  description: >-\n    impact.com's \"Building with LLMs\" guide states that multi-customer apps follow OAuth 2.0\n    Authorization Code + PKCE with documented token rotation. No OAuth endpoints, scopes or\n    registration flow were located on the public developer portal in this pass, and no oauth2\n    securityScheme appears in any of the 67 published specs — so this is recorded as documented\n    but not machine-readable.\n  sources: [docs]\nbase_urls:\n  brand: https://api.impact.com/Advertisers/{AccountSID}/\n  partner: https://api.impact.com/MediaPartners/{AccountSID}/\n  agency: https://api.impact.com/Agencies/{AccountSID}/\n  advocate: https://app.referralsaasquatch.com/api/v1/{tenant_alias}/\n  mcp:\
  \ https://mcp.impact.com/mcp\ncredential_handling:\n  guidance_published: true\n  detail: >-\n    The docs tell integrators never to hardcode secrets, to store them in a vault or encrypted\n    environment variables, to start with read-only scopes, and to promote separate tokens per\n    environment (development / staging / production). They also tell users to redact Account SID,\n    Auth Token, OAuth tokens, bearer tokens and customer identifiers before pasting doc examples\n    into third-party assistants.\n  rotation: Tokens can be rotated, duplicated, disabled and deleted from the token detail page.\nnotes: >-\n  Upgraded from the 2026-07-19 pass. Scheme names, counts and header names are now cross-checked\n  against the 67 harvested OpenAPI documents rather than the docs alone, which surfaced the\n  Advocate UserJWT header that the prose pages describe but do not name.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/impact-radius/refs/heads/main/authentication/impact-radius-authentication.yml
summary_line: http/apiKey · 6 schemes
tags:
- Company
- Partnership Management
- Affiliate Marketing
- Influencer Marketing
- Referral Marketing
- Attribution
- Martech
- Advocate
- Creator Economy
- E-Commerce
---

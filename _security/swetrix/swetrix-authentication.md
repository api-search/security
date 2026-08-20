---
api_key_in:
- header
api_specs:
- filename: swetrix-events-api-openapi.yml
  format: yaml
  label: Swetrix Events API
  slug: swetrix-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swetrix/refs/heads/main/openapi/swetrix-events-api-openapi.yml
- filename: swetrix-annotations-api-openapi.yml
  format: yaml
  label: Swetrix Annotations API
  slug: swetrix-annotations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swetrix/refs/heads/main/openapi/swetrix-annotations-api-openapi.yml
- filename: swetrix-custom-events-api-openapi.yml
  format: yaml
  label: Swetrix Custom Events API
  slug: swetrix-custom-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swetrix/refs/heads/main/openapi/swetrix-custom-events-api-openapi.yml
- filename: swetrix-errors-api-openapi.yml
  format: yaml
  label: Swetrix Errors API
  slug: swetrix-errors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swetrix/refs/heads/main/openapi/swetrix-errors-api-openapi.yml
- filename: swetrix-feature-flags-api-openapi.yml
  format: yaml
  label: Swetrix Feature Flags API
  slug: swetrix-feature-flags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swetrix/refs/heads/main/openapi/swetrix-feature-flags-api-openapi.yml
- filename: swetrix-funnels-api-openapi.yml
  format: yaml
  label: Swetrix Funnels API
  slug: swetrix-funnels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swetrix/refs/heads/main/openapi/swetrix-funnels-api-openapi.yml
- filename: swetrix-organisations-api-openapi.yml
  format: yaml
  label: Swetrix Organisations API
  slug: swetrix-organisations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swetrix/refs/heads/main/openapi/swetrix-organisations-api-openapi.yml
- filename: swetrix-performance-api-openapi.yml
  format: yaml
  label: Swetrix Performance API
  slug: swetrix-performance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swetrix/refs/heads/main/openapi/swetrix-performance-api-openapi.yml
- filename: swetrix-projects-api-openapi.yml
  format: yaml
  label: Swetrix Projects API
  slug: swetrix-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swetrix/refs/heads/main/openapi/swetrix-projects-api-openapi.yml
- filename: swetrix-revenue-api-openapi.yml
  format: yaml
  label: Swetrix Revenue API
  slug: swetrix-revenue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swetrix/refs/heads/main/openapi/swetrix-revenue-api-openapi.yml
- filename: swetrix-sessions-api-openapi.yml
  format: yaml
  label: Swetrix Sessions API
  slug: swetrix-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swetrix/refs/heads/main/openapi/swetrix-sessions-api-openapi.yml
- filename: swetrix-traffic-api-openapi.yml
  format: yaml
  label: Swetrix Traffic API
  slug: swetrix-traffic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swetrix/refs/heads/main/openapi/swetrix-traffic-api-openapi.yml
- filename: swetrix-views-api-openapi.yml
  format: yaml
  label: Swetrix Views API
  slug: swetrix-views-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swetrix/refs/heads/main/openapi/swetrix-views-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Swetrix Authentication
name_suffix: Authentication
oauth_flows: []
overview: Swetrix secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Swetrix
provider_slug: swetrix
scheme_count: 1
schemes:
- description: API key from Swetrix account settings (https://swetrix.com/user-settings)
  in: header
  name: ApiKeyAuth
  parameter: X-Api-Key
  sources:
  - openapi/swetrix-admin-api-openapi.yml
  - openapi/swetrix-events-api-openapi.yml
  - openapi/swetrix-statistics-api-openapi.yml
  type: apiKey
slug: swetrix-authentication
source_filename: swetrix-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/*.yml (derived baseline)\ndocs: https://swetrix.com/docs/settings/api-keys\nsearched_sources:\n  - https://swetrix.com/docs/settings/api-keys\n  - https://swetrix.com/docs/statistics-api\n  - https://swetrix.com/docs/api/stats-v2\n  - https://swetrix.com/docs/events-api\n  - https://swetrix.com/security\nsummary:\n  types:\n    - apiKey\n  api_key_in:\n    - header\n  oauth2: false\n  oidc: false\n  note: >-\n    Swetrix is API-key only. There is no OAuth, no OIDC and no scope surface —\n    /.well-known/openid-configuration and /.well-known/oauth-authorization-server\n    return 404 on every host (probed 2026-08-13), so scopes/ is deliberately not\n    written for this provider.\nschemes:\n  - name: ApiKeyAuth\n    type: apiKey\n    in: header\n    parameter: X-Api-Key\n    description: API key from Swetrix account settings (https://swetrix.com/user-settings)\n    sources:\n      - openapi/swetrix-admin-api-openapi.yml\n\
  \      - openapi/swetrix-events-api-openapi.yml\n      - openapi/swetrix-statistics-api-openapi.yml\nkey_management:\n  issuance: >-\n    Account Settings → Account tab → API key section → \"Generate API key\". The\n    key is displayed once on creation.\n  count_per_account: one\n  rotation: >-\n    Delete and regenerate. Deleting immediately breaks every application or\n    script using the key — there is no overlap window and no second active key,\n    so rotation is a hard cutover.\n  revocation: Account Settings → API key → \"Delete API key\" with modal confirmation.\n  scoping: >-\n    None. A key carries the full rights of the account that owns it, across every\n    project that account can reach. There is no read-only key, no per-project key\n    and no expiry.\n  prefix: none published\n  test_keys: >-\n    None — Swetrix has no test/live key separation. See\n    sandbox/swetrix-sandbox.yml.\n  guidance: >-\n    \"Treat API keys like passwords. Keep them secret, do not hardcode\
  \ them, and\n    do not share them.\"\n  docs: https://swetrix.com/docs/settings/api-keys\nanonymous_access:\n  supported: true\n  conditions:\n    - >-\n      Public projects can be queried through the Statistics API (v1 and v2)\n      without an API key. The v1 reference states requests without a valid key\n      fail \"except for the publicly available API endpoints\"; the v2 reference\n      states \"Public projects can be queried without a key.\"\n    - >-\n      Event ingestion (POST /log, /log/custom, /log/hb, /log/error) is\n      unauthenticated by design — the tracking script runs in a visitor's\n      browser and carries only the project id.\n  exception: >-\n    POST /log/revenue is server-side only and REQUIRES an API key whose account\n    has rights on the target project; a key without them returns 403.\naccount_security:\n  two_factor: supported (https://swetrix.com/docs/settings/2-factor-authentication)\n  sso:\n    supported: true\n    note: >-\n      Native SSO is referenced\
  \ on the security page; SAML-based SSO is listed as\n      an Enterprise-tier entitlement on the pricing comparison.\n  password_storage: bcrypt (hashed and salted), per https://swetrix.com/security\n  token_storage: >-\n    Integration tokens (Google Search Console OAuth, Paddle/Stripe revenue keys)\n    are encrypted at rest with AES-256-CBC and Rabbit.\ntransport:\n  https_required: true\n  hsts: true\n  hsts_max_age: 31536000\n  tls: TLSv1.3\n  evidence: security/swetrix-domain-security.yml\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swetrix/refs/heads/main/authentication/swetrix-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Analytics
- Cookieless Tracking
- GDPR Compliant
- Open-Source
- Privacy
- Real-Time Analytics
- Web Analytics
---

---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Moda Operandi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Moda Operandi declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Moda Operandi
provider_slug: moda-operandi
scheme_count: 0
schemes: []
slug: moda-operandi-authentication
source_filename: moda-operandi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: https://search.modaoperandi.com/graphql\nnote: >-\n  Moda Operandi publishes no authentication documentation, because it publishes no developer\n  program. This profile is what was OBSERVED against the live GraphQL endpoint, not what the\n  provider claims. There is no OpenAPI securityScheme to derive from.\nsummary:\n  types: []\n  api_key_in: []\n  oauth2_flows: []\n  anonymous_access: true\nschemes: []\nobserved:\n- surface: https://search.modaoperandi.com/graphql\n  transport: https\n  requires_credentials: false\n  evidence: >-\n    An unauthenticated POST of the full GraphQL IntrospectionQuery returned HTTP 200 with a\n    complete __schema (121 types). An unauthenticated POST of \"{ version }\" returned\n    {\"data\":{\"version\":2}}. No Authorization header, cookie or API key was sent.\n  in_schema:\n    - field: user_token\n      type: String\n      note: >-\n        A Query field that returns a token string. Its purpose\
  \ is not documented; it appears to\n        issue an Algolia/analytics session identifier rather than an authorization credential.\n        Not probed for a value.\n    - field: usage_stats\n      args: [token]\n      note: >-\n        Takes a required `token` argument, which implies a privileged surface exists behind some\n        token scheme. No token issuance, scope or format is documented anywhere public.\n- surface: https://api.modaoperandi.com/public\n  transport: https\n  requires_credentials: unknown\n  evidence: >-\n    Named as MODA_API_URL in the storefront runtime config. Every anonymously probed path under\n    this host returned HTTP 404 with a zero-byte body, including /public itself. No auth challenge\n    was ever emitted, so nothing about its auth model could be established.\ngaps:\n- No published authentication documentation.\n- No OAuth 2.0 or OpenID Connect discovery document on any host (see well-known/).\n- The token accepted by `usage_stats` has no documented issuance\
  \ path.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moda-operandi/refs/heads/main/authentication/moda-operandi-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Retail
- E-Commerce
- Fashion
- Luxury
- Marketplace
- Apparel
- Search
- GraphQL
- Product Catalog
---

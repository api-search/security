---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Hnry Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hnry declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Hnry
provider_slug: hnry
scheme_count: 0
schemes: []
slug: hnry-authentication
source_filename: hnry-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: >-\n  live probes of https://app.hnry.io/api-docs, https://app.hnry.io/oauth/authorize and\n  https://zapier.com/apps/hnry/integrations\nnote: >-\n  DERIVED FROM PROBES, NOT FROM PROVIDER DOCUMENTATION. Hnry publishes no public authentication\n  reference: the API reference at app.hnry.io/api-docs is behind HTTP Basic, and the Hnry help\n  centre article that explains connecting Hnry to Zapier also returns 401. Everything below is\n  what was observable anonymously from the live platform plus the published Zapier listing.\n  Nothing here is a quoted Hnry statement about its own auth model, and no scheme names, header\n  names, token formats or scopes are asserted, because none are published.\nobserved:\n- surface: API reference\n  url: https://app.hnry.io/api-docs\n  status: 401\n  scheme: HTTP Basic\n  detail: >-\n    Responds `WWW-Authenticate: Basic realm=\"\"` with an empty body. The whole /api-docs/* tree\n    behaves identically\
  \ (/api-docs/, /api-docs/index.html, /api-docs/swagger.json,\n    /api-docs/openapi.json all 401), so the documentation itself — not just the API — is\n    credential-gated. The same behaviour is present on the UAT host, https://uat.hnry.io/api-docs.\n- surface: OAuth authorization endpoint\n  url: https://app.hnry.io/oauth/authorize\n  status: 302\n  location: https://app.hnry.io/users/sign_in?mode=api\n  detail: >-\n    A live /oauth/authorize route exists and redirects anonymous callers to an API-mode sign-in.\n    The `?mode=api` parameter and the Rails/Doorkeeper-shaped path are consistent with an\n    authorization-code flow, but /oauth/token and /oauth/applications both return 404 anonymously\n    and no client-registration, scope or grant-type documentation is published, so the flow cannot\n    be characterised further without credentials.\n- surface: Zapier integration\n  url: https://zapier.com/apps/hnry/integrations\n  status: 200\n  detail: >-\n    Hnry ships a public, non-beta\
  \ Zapier app in the Accounting category. A Zapier app requires a\n    working authentication mechanism against the Hnry API, and Hnry's own help centre documents\n    connecting an account, but that article (help.hnry.io/en/articles/5094374) returns 401, so the\n    credential type Zapier collects could not be confirmed from a Hnry-published source.\noauth:\n  discovery_document: null\n  discovery_probe:\n    url: https://app.hnry.io/.well-known/oauth-authorization-server\n    status: 404\n  scopes_published: false\nmtls: false\npublic_signup_for_api_access: false\npublic_signup_note: >-\n  There is no developer signup, sandbox key issuance or API-key self-service page. API access is a\n  property of a funded Hnry customer account (https://app.hnry.io/signup/jurisdiction_selection).\ngaps:\n- No public authentication reference — the auth documentation is behind the same wall as the API.\n- No /.well-known/oauth-authorization-server or /.well-known/openid-configuration on any host.\n- No\
  \ published scopes, token lifetimes, rotation policy or key-prefix convention.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hnry/refs/heads/main/authentication/hnry-authentication.yml
summary_line: 0 schemes
tags:
- Accounting
- Tax
- Payments
- Invoicing
- Expense Management
- Financial-Services
- Sole Traders
- Payroll
- Fintech
- New Zealand
- Australia
- United Kingdom
---

---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Sniffcat Authentication
name_suffix: Authentication
oauth_flows: []
overview: SniffCat declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: SniffCat
provider_slug: sniffcat
scheme_count: 1
schemes:
- applies_to: all endpoints (/api/v1/blacklist, /check, /reports, /report, /bulk)
  description: Static per-account API token. "All endpoints require the X-Secret-Token header. You can generate a token at /api." — https://sniffcat.com/documentation/api
  expiry: not documented
  id: secretToken
  in: header
  issuance:
    note: The token page is behind the session login; probing https://sniffcat.com/api anonymously returns the SniffCat login screen (HTTP 200, login form). Registration is self-serve at https://sniffcat.com/register.
    requires_login: true
    url: https://sniffcat.com/api
  name: X-Secret-Token
  prefix: null
  required: true
  rotation: not documented
  type: apiKey
slug: sniffcat-authentication
source_filename: sniffcat-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: searched\nsource: https://sniffcat.com/documentation/api\ndocs: https://sniffcat.com/documentation/api\nprobe:\n  url: https://api.sniffcat.com/api/v1/check?ip=1.1.1.1\n  date: '2026-08-19'\n  status: 403\n  body: '{\"success\":false,\"status\":403,\"message\":\"Missing API token in request headers.\"}'\n  note: >-\n    Derived from a live unauthenticated call, not from a spec — SniffCat publishes no OpenAPI, so\n    there are no securitySchemes to parse. The 403 body confirms the header is mandatory on every\n    endpoint.\nsummary: >-\n  A single authentication mechanism across the whole API: a static, account-scoped bearer-style\n  secret sent in a custom `X-Secret-Token` request header. No OAuth 2.0, no OpenID Connect, no\n  mutual TLS, no HTTP Basic, no signed requests, and no scope system — entitlement is expressed\n  through account ROLES that set daily quotas rather than through token scopes.\nschemes:\n- id: secretToken\n  type: apiKey\n\
  \  in: header\n  name: X-Secret-Token\n  applies_to: all endpoints (/api/v1/blacklist, /check, /reports, /report, /bulk)\n  required: true\n  description: >-\n    Static per-account API token. \"All endpoints require the X-Secret-Token header. You can generate\n    a token at /api.\" — https://sniffcat.com/documentation/api\n  issuance:\n    url: https://sniffcat.com/api\n    requires_login: true\n    note: >-\n      The token page is behind the session login; probing https://sniffcat.com/api anonymously\n      returns the SniffCat login screen (HTTP 200, login form). Registration is self-serve at\n      https://sniffcat.com/register.\n  prefix: null\n  rotation: not documented\n  expiry: not documented\noauth2: false\nopenid_connect: false\nmutual_tls: false\nhttp_basic: false\nrequest_signing: false\nscopes:\n  supported: false\n  note: >-\n    No scope or permission strings exist. Authorization granularity is per-ROLE daily quota per\n    operation — see rate-limits/sniffcat-rate-limits.yml\
  \ and https://sniffcat.com/documentation/roles.\nauthorization_model:\n  type: role-based-quota\n  roles:\n  - {name: Individual, trust_level: 1}\n  - {name: Early User, trust_level: 1.19}\n  - {name: Webmaster, trust_level: 1.24}\n  - {name: Contributor, trust_level: 1.36}\n  - {name: SniffCat Enthusiast, trust_level: 1.48}\n  - {name: Hosting Provider, trust_level: 1.54}\n  - {name: ISP, trust_level: 1.62}\n  - {name: Security Researcher, trust_level: 1.75}\n  - {name: Law Enforcement, trust_level: 1.83}\n  note: >-\n    Roles are additive — a user may hold several. Trust level also weights the impact of that user's\n    submitted reports on an IP's abuse confidence score, so the role is an authorization control AND\n    a data-quality control.\nfailure_modes:\n- status: 403\n  condition: X-Secret-Token header absent\n  body: '{\"success\":false,\"status\":403,\"message\":\"Missing API token in request headers.\"}'\n  method: probed\n- status: 403\n  condition: token valid but the account's\
  \ role grants no quota for that operation\n  documented_as: No quota assigned to the role / No limits configured for this role\n  source: https://sniffcat.com/documentation/api/blacklist, https://sniffcat.com/documentation/api/check\n- status: 429\n  condition: daily role quota or the 400-req/120s edge window exhausted\ntransport:\n  https_only: true\n  hsts: 'max-age=31536000; includeSubDomains; preload'\n  tls_version: TLSv1.3\ngaps:\n- No documented token rotation, revocation or expiry policy.\n- No token prefix convention, so a leaked SniffCat token is not self-identifying to a secret scanner.\n- No scopes, so a token minted for read-only blacklist consumption can also submit abuse reports.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sniffcat/refs/heads/main/authentication/sniffcat-authentication.yml
summary_line: 1 scheme
tags:
- threat-intelligence
- ip-reputation
- abuse-database
- cybersecurity
- osint
- network-security
- sysadmin-tools
- blocklist
- abuse-reporting
- ip-blocklist
- ip-intelligence
- threat-feeds
---

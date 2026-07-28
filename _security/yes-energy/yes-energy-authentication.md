---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: probed
name: Yes Energy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Yes Energy secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Yes Energy
provider_slug: yes-energy
scheme_count: 1
schemes:
- credential_issuance: Commercial subscription only. There is no self-serve signup, no free tier, no API-key console, and no sandbox. The published entry paths are the demo request form (https://www.yesenergy.com/demo), support@yesenergy.com, and +1 303-993-2773. Credentials appear to be the customer's PowerSignals account username/password.
  evidence: 'curl -I https://services.yesenergy.com/PS/rest/ -> HTTP/2 401 with `www-authenticate: Basic realm="Realm"` (probed 2026-07-27); the same services.yesenergy.com/PS security realm fronts the PowerSignals web application login at /PS/security/login.'
  in: header
  name: basicAuth
  parameter: Authorization
  realm: Realm
  scheme: basic
  transport: https
  type: http
slug: yes-energy-authentication
source_filename: yes-energy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: >-\n  Live anonymous probe of https://services.yesenergy.com/PS/rest/ (HTTP 401 with\n  a WWW-Authenticate challenge), plus /.well-known/ discovery probes on the same\n  host. No OpenAPI security schemes exist to derive from — Yes Energy publishes\n  no machine-readable specification.\nsummary:\n  types:\n  - http\n  api_key_in: []\n  oauth2_flows: []\n  notes: >-\n    Single auth mechanism. HTTP Basic over TLS 1.3, credentials issued only to\n    contracted subscribers. No API-key header scheme, no OAuth 2.0, no OpenID\n    Connect, and no mutual TLS is published or discoverable.\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  realm: Realm\n  in: header\n  parameter: Authorization\n  transport: https\n  evidence: >-\n    curl -I https://services.yesenergy.com/PS/rest/ -> HTTP/2 401 with\n    `www-authenticate: Basic realm=\"Realm\"` (probed 2026-07-27); the same\n    services.yesenergy.com/PS security realm fronts\
  \ the PowerSignals web\n    application login at /PS/security/login.\n  credential_issuance: >-\n    Commercial subscription only. There is no self-serve signup, no free tier,\n    no API-key console, and no sandbox. The published entry paths are the demo\n    request form (https://www.yesenergy.com/demo), support@yesenergy.com, and\n    +1 303-993-2773. Credentials appear to be the customer's PowerSignals\n    account username/password.\nnegative_findings:\n- check: OpenID Connect discovery\n  result: not served\n  evidence: https://services.yesenergy.com/.well-known/openid-configuration -> 404\n- check: OAuth 2.0 authorization server metadata (RFC 8414)\n  result: not served\n  evidence: https://services.yesenergy.com/.well-known/oauth-authorization-server -> 404\n- check: OAuth 2.0 protected resource metadata (RFC 9728)\n  result: not served\n  evidence: https://services.yesenergy.com/.well-known/oauth-protected-resource -> 404\n- check: Public authentication documentation\n  result:\
  \ gated\n  evidence: >-\n    https://help.yesenergy.com/ 301 -> /help, 302 ->\n    services.yesenergy.com/PS/KnowledgeOwlAuthentication, 302 ->\n    /PS/security/login, terminating in HTTP 401. The auth reference is inside a\n    login-gated KnowledgeOwl knowledge base.\nscopes: []\nscopes_note: >-\n  Not applicable. HTTP Basic has no scope surface; entitlement is enforced by\n  the subscription package attached to the account, not by a token scope.\nrelated:\n- security/yes-energy-domain-security.yml\n- conventions/yes-energy-conventions.yml\n- well-known/yes-energy-well-known.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yes-energy/refs/heads/main/authentication/yes-energy-authentication.yml
summary_line: http · 1 scheme
tags:
- Energy
- United States
- Energy Markets
- Electricity
- Grid
- Market Data
- Wholesale Power
- ISO RTO
- Renewables
- Trading
---

---
api_key_in:
- header
api_specs:
- filename: hacknotice-openapi.yml
  format: yaml
  label: HackNotice API
  slug: hacknotice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hacknotice/refs/heads/main/openapi/hacknotice-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Hacknotice Authentication
name_suffix: Authentication
oauth_flows: []
overview: HackNotice secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: HackNotice
provider_slug: hacknotice
scheme_count: 3
schemes:
- description: 'Session token from POST /auth/sign_in, sent as the literal prefix "JWT " followed by the token — e.g. Authorization: JWT <token>. Note this is HackNotice''s own scheme, not RFC 6750 Bearer.'
  in: header
  name: jwtAuth
  parameter: Authorization
  sources:
  - openapi/hacknotice-openapi.yml
  type: apiKey
- description: Per-account API key issued by HackNotice, sent in the lower-case "apikey" header alongside the JWT on most operations.
  in: header
  name: apiKeyAuth
  parameter: apikey
  sources:
  - openapi/hacknotice-openapi.yml
  type: apiKey
- description: Per-user HackNotice integration secret (hn_ik_ prefix). Single-header alternative to apikey + email + password; also the credential used by the HackNotice MCP server.
  in: header
  name: integrationKeyAuth
  parameter: X-HackNotice-Integration-Key
  sources:
  - openapi/hacknotice-openapi.yml
  type: apiKey
slug: hacknotice-authentication
source_filename: hacknotice-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: searched\nsource:\n- https://api-docs.hacknotice.com (HackNotice-API collection description)\n- https://github.com/HackNotice/n8n-nodes-hacknotice — credentials/HackNoticeApi.credentials.ts\n- https://github.com/HackNotice/n8n-nodes-hacknotice-mcp — credentials/HackNoticeMcpApi.credentials.ts\n- openapi/hacknotice-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  note: 'Three header API-key schemes, no OAuth 2.0 and no OpenID Connect. /.well-known/openid-configuration and\n    /.well-known/oauth-authorization-server both return 404 on api.hacknotice.com, and the MCP host returns 404\n    on both OAuth metadata paths. There is therefore no scopes/ artifact for this provider: with no OAuth surface\n    there is no scope model to derive.'\nschemes:\n- name: jwtAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Session token from POST /auth/sign_in, sent as the literal prefix\
  \ \"JWT \" followed by the token —\n    e.g. Authorization: JWT <token>. Note this is HackNotice''s own scheme, not RFC 6750 Bearer.'\n  sources:\n  - openapi/hacknotice-openapi.yml\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: apikey\n  description: Per-account API key issued by HackNotice, sent in the lower-case \"apikey\" header alongside the JWT\n    on most operations.\n  sources:\n  - openapi/hacknotice-openapi.yml\n- name: integrationKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-HackNotice-Integration-Key\n  description: Per-user HackNotice integration secret (hn_ik_ prefix). Single-header alternative to apikey + email\n    + password; also the credential used by the HackNotice MCP server.\n  sources:\n  - openapi/hacknotice-openapi.yml\ndocs: https://api-docs.hacknotice.com\nflows:\n- name: apiKey + email + password\n  steps:\n  - POST /auth/sign_in with form fields email and password, sending the apikey header\n  - POST /auth/twofa_sign_in instead when\
  \ the account has 2FA enabled\n  - 'Send the returned token on every subsequent call as Authorization: JWT <token>'\n  - GET /auth/sign_out or /auth/sign_out_all to end sessions\n  token: JWT (RFC 7519) carrying email, customer_id, _id, iat and exp claims. Tenant scoping is inside the token\n    — customer_id is never passed as a parameter.\n  gotcha: The literal prefix is \"JWT \", not \"Bearer \". HackNotice calls this out explicitly in its own documentation.\n    A standard RFC 6750 Bearer client fails with 401 and no explanation.\n- name: integration key\n  steps:\n  - 'Send X-HackNotice-Integration-Key: hn_ik_... on every request. No sign-in round trip.'\n  token: Opaque per-user secret, hn_ik_ prefix.\n  note: Same credential the HackNotice MCP server validates on every tools/call.\ntwo_factor:\n  supported: true\n  operation: post2FaSignIn (POST /auth/twofa_sign_in)\nsso:\n  saml2: true\n  providers:\n  - Microsoft Entra ID (Azure AD)\n  - Okta\n  docs:\n  - https://hacknotice.zendesk.com/hc/en-us/articles/16860907619860-Microsoft-Azure-AD-EntraID-SAML-SSO-Integration\n\
  \  - https://hacknotice.zendesk.com/hc/en-us/articles/16860841528724-OKTA-SAML-Integration\n  note: Platform sign-in only. SAML does not mint an API credential.\naccess_gate:\n  approved_accounts_only: true\n  consultation_required: 30 minutes, before API usage\n  source: https://hacknotice.zendesk.com/hc/en-us/articles/13540425661844-API\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hacknotice/refs/heads/main/authentication/hacknotice-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Company
- Security
- Threat Intelligence
- Cybersecurity
- Dark Web Monitoring
- Data Breaches
- Credential Monitoring
- Third Party Risk
- Vendor Risk Management
- Vulnerability Management
- Ransomware
- Security Assessments
- Alerts
- Monitoring
---

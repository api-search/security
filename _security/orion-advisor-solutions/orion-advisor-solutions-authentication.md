---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: orion-advisor-solutions-orion-connect-openapi.json
  format: json
  label: Orion API
  slug: orion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orion-advisor-solutions/refs/heads/main/openapi/orion-advisor-solutions-orion-connect-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Orion Advisor Solutions Authentication
name_suffix: Authentication
oauth_flows: []
overview: Orion Advisor Solutions secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Orion Advisor Solutions
provider_slug: orion-advisor-solutions
scheme_count: 1
schemes:
- description: 'JWT Authorization header using the Session scheme. Example: "Authorization: Session {token}"'
  in: header
  name: Authorization
  parameter: Authorization
  sources:
  - openapi/orion-advisor-solutions-orion-connect-openapi.json
  type: apiKey
slug: orion-advisor-solutions-authentication
source_filename: orion-advisor-solutions-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-10'\nmethod: searched\nsource: openapi/orion-advisor-solutions-orion-connect-openapi.json\ndocs: https://developers.orionadvisor.com/guides/authentication-third-party-website/\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  flows:\n  - basic-to-session-token\n  - impersonation\n  - oauth-token-exchange\n  - saml-2.0-sso\nschemes:\n- name: Authorization\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'JWT Authorization header using the Session scheme. Example: \"Authorization:\n    Session {token}\"'\n  sources:\n  - openapi/orion-advisor-solutions-orion-connect-openapi.json\nflows:\n- flow: basic-to-session-token\n  detail: 'GET https://api.orionadvisor.com/api/v1/security/token with\n    \"Authorization: Basic {base64(uid:pwd)}\" using Orion service-level credentials\n    (created by Orion Tech Support) returns an auth token, sent on subsequent calls\n    as \"Authorization: Session {token}\".'\n  operation: openapi/orion-advisor-solutions-orion-connect-openapi.json#Token_GetTokenAsync\n\
  - flow: impersonation\n  detail: 'GET /v1/Security/Token with \"Authorization: Impersonate {service_token}\"\n    plus \"Entity: 5\" (Household) and \"EntityId: {HouseholdId}\" headers returns an\n    auth token impersonated as the specified household — for partners acting on\n    behalf of an end user.'\n- flow: oauth-token-exchange\n  detail: POST /v1/Security/Token (Token_GetTokenForOAuthAsync) supports the OAuth\n    framework; partners integrating on behalf of an end user can acquire a\n    long-lived refresh token. Full flow docs are behind the OrionConnect login.\n  operation: openapi/orion-advisor-solutions-orion-connect-openapi.json#Token_GetTokenForOAuthAsync\n- flow: saml-2.0-sso\n  detail: SAML 2.0 SSO for contextual sign-on into Orion and partner sites\n    (https://developers.orionadvisor.com/guides/contextual-sso-into-orion/).\ncredentials:\n  provisioning: On request — Orion technical contact or SME-Integrations@orion.com;\n    https://developers.orionadvisor.com/creds-request/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orion-advisor-solutions/refs/heads/main/authentication/orion-advisor-solutions-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- wealth-management
- fintech
- financial-advisors
- portfolio-accounting
- trading-rebalancing
- financial-planning
- billing
- reporting
- risk
- RIA-technology
---

---
api_key_in:
- header
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Check Technologies Authentication
name_suffix: Authentication
oauth_flows: []
overview: Check Technologies secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Check Technologies
provider_slug: check-technologies
scheme_count: 2
schemes:
- description: All API requests authenticate with an Authorization header carrying a Bearer token (the API key). API keys are issued per environment (sandbox vs production). Keys can be scoped with optional IP restrictions for an extra layer of security.
  format: 'Authorization: Bearer <API_KEY>'
  header: Authorization
  in: header
  name: bearerAuth
  scheme: bearer
  type: http
- description: Ecosystem Partners integrate via an OAuth flow to gain scoped access to partner companies' Check data (see the Ecosystem Partner Guide).
  docs: https://docs.checkhq.com/docs/check-oauth-integrations
  name: ecosystemPartnerOAuth
  type: oauth2
slug: check-technologies-authentication
source_filename: check-technologies-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.checkhq.com/reference/authentication\ndocs: https://docs.checkhq.com/reference/authentication\nsummary:\n  types: [http, oauth2]\n  http_scheme: bearer\n  api_key_in: [header]\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Authorization: Bearer <API_KEY>'\n  description: >-\n    All API requests authenticate with an Authorization header carrying a\n    Bearer token (the API key). API keys are issued per environment\n    (sandbox vs production). Keys can be scoped with optional IP restrictions\n    for an extra layer of security.\n- name: ecosystemPartnerOAuth\n  type: oauth2\n  description: >-\n    Ecosystem Partners integrate via an OAuth flow to gain scoped access to\n    partner companies' Check data (see the Ecosystem Partner Guide).\n  docs: https://docs.checkhq.com/docs/check-oauth-integrations\nmcp_auth:\n  description: >-\n    The hosted\
  \ Check MCP server uses browser-based OAuth via Check Console\n    login instead of static API keys.\n  docs: https://docs.checkhq.com/docs/hosted-remote\nextras:\n  ip_restrictions: supported\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/check-technologies/refs/heads/main/authentication/check-technologies-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Payroll
- Embedded Finance
- Fintech
- Payments
- Human Resources
- Tax
- Compliance
- Developer Tools
- API
---

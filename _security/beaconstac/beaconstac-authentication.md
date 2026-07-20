---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Beaconstac Authentication
name_suffix: Authentication
oauth_flows: []
overview: Beaconstac secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Beaconstac
provider_slug: beaconstac
scheme_count: 2
schemes:
- description: A dashboard-issued API key sent as a Token in the Authorization header. Requests also require an Organization ID (obtained from the Uniqode dashboard's API section) to scope the account. No OAuth2 flow is exposed for the public REST API.
  format: 'Authorization: Token <API_KEY>'
  in: header
  name: TokenAuth
  parameter_name: Authorization
  sources:
  - https://apidocs.uniqode.com/
  type: apiKey
- description: Organization identifier obtained from the dashboard API section, sent alongside the token.
  in: header
  name: OrganizationId
  parameter_name: Organization-Id
  sources:
  - https://www.uniqode.com/qr-code-generator/api
  type: apiKey
slug: beaconstac-authentication
source_filename: beaconstac-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://apidocs.uniqode.com/, https://www.uniqode.com/qr-code-generator/api\ndocs: https://apidocs.uniqode.com/\n# Derived from the published API documentation (no OpenAPI available to mechanically derive).\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n- name: TokenAuth\n  type: apiKey\n  in: header\n  parameter_name: Authorization\n  format: \"Authorization: Token <API_KEY>\"\n  description: >-\n    A dashboard-issued API key sent as a Token in the Authorization header. Requests also\n    require an Organization ID (obtained from the Uniqode dashboard's API section) to scope\n    the account. No OAuth2 flow is exposed for the public REST API.\n  sources: [https://apidocs.uniqode.com/]\n- name: OrganizationId\n  type: apiKey\n  in: header\n  parameter_name: Organization-Id\n  description: Organization identifier obtained from the dashboard API section, sent alongside the token.\n  sources:\
  \ [https://www.uniqode.com/qr-code-generator/api]\nnotes:\n- End-user account access to the Uniqode dashboard additionally supports 2FA and SAML-based SSO (Auth0 is the identity subprocessor); these govern dashboard/SSO login, not the REST API token.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beaconstac/refs/heads/main/authentication/beaconstac-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Big Data
- QR Codes
- Digital Business Cards
- Marketing
- Analytics
- SaaS
- Proximity
---

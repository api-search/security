---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Zenoti Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zenoti declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Zenoti
provider_slug: zenoti
scheme_count: 2
schemes:
- expiry: Does not expire (rotate/revoke manually)
  format: apikey {api_key}
  id: apiKey
  in: header
  name: Authorization
  recommended_for: Server-side integrations
  scope: Global master data; no API restrictions
  type: apiKey
- format: bearer {access_token}
  id: bearerToken
  in: header
  invalidation: Employee access tokens expire when the employee password changes or the employee leaves the organization.
  name: Authorization
  recommended_for: Client-side / per-user (guest, therapist) interactions
  refresh:
    behavior: Refreshing deactivates existing access tokens and issues a new one.
    endpoints:
    - Generate an access token
    - Refresh an access token
    - Revoke an existing access token
    refresh_token_lifetime: 90 days (single use)
  scheme: bearer
  scope: Module- or role-based data, restricted by app user role
  token_lifetime: Access token valid 24 hours
  type: http
slug: zenoti-authentication
source_filename: zenoti-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.zenoti.com/docs/authentication.md\ndocs: https://docs.zenoti.com/docs/authentication.md\nsummary: >-\n  Zenoti API supports two authentication types: API-key based (global master\n  data, no expiry, server-side) and access-token (bearer) based (module /\n  role-scoped, expiring, client-side). Both are supplied in the Authorization\n  request header.\nschemes:\n- id: apiKey\n  type: apiKey\n  in: header\n  name: Authorization\n  format: 'apikey {api_key}'\n  scope: Global master data; no API restrictions\n  expiry: Does not expire (rotate/revoke manually)\n  recommended_for: Server-side integrations\n- id: bearerToken\n  type: http\n  scheme: bearer\n  in: header\n  name: Authorization\n  format: 'bearer {access_token}'\n  scope: Module- or role-based data, restricted by app user role\n  recommended_for: Client-side / per-user (guest, therapist) interactions\n  token_lifetime: Access token valid 24 hours\n  refresh:\n\
  \    refresh_token_lifetime: 90 days (single use)\n    behavior: >-\n      Refreshing deactivates existing access tokens and issues a new one.\n    endpoints:\n    - Generate an access token\n    - Refresh an access token\n    - Revoke an existing access token\n  invalidation: >-\n    Employee access tokens expire when the employee password changes or the\n    employee leaves the organization.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zenoti/refs/heads/main/authentication/zenoti-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Services
- Beauty
- Wellness
- Spa
- Salon
- Fitness
- Booking
- Payments
- Software-as-a-Service
---

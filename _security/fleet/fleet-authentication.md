---
api_key_in:
- header
api_specs:
- filename: fleet-premium-openapi.json
  format: json
  label: Fleet REST API
  slug: fleet-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleet/refs/heads/main/openapi/fleet-premium-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Fleet Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fleet secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Fleet
provider_slug: fleet
scheme_count: 2
schemes:
- format: Bearer <token>
  header: Authorization
  in: header
  name: bearerToken
  obtained_via:
  - description: Email + password login returning a user object and session token.
    endpoint: POST /api/v1/fleet/login
  - description: Required for SSO/MFA users; API login is disabled for them.
    ui: /profile ("My account" > Get API token)
  scheme: bearer
  sources:
  - docs
  type: http
- description: Non-expiring token issued to an API-only user (fleetctl user create --api-only) for automation and GitOps workflows.
  header: Authorization
  in: header
  name: apiOnlyUserToken
  scheme: bearer
  sources:
  - docs
  type: http
slug: fleet-authentication
source_filename: fleet-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://fleetdm.com/docs/rest-api/rest-api#authentication\ndocs: https://fleetdm.com/docs/rest-api/rest-api#authentication\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  api_key_in: [header]\n  oauth2_flows: []\n  notes: >-\n    Fleet's REST API uses bearer-token authentication. Tokens are obtained by\n    POST /api/v1/fleet/login (email + password) or, for SSO/MFA users, from the\n    \"My account\" page in the Fleet UI (\"Get API token\"). API-only users are the\n    recommended pattern for automation because their tokens do not expire, unlike\n    regular user session tokens which expire frequently. SSO is supported for\n    human login (SAML/OIDC IdPs).\nschemes:\n  - name: bearerToken\n    type: http\n    scheme: bearer\n    in: header\n    header: Authorization\n    format: 'Bearer <token>'\n    obtained_via:\n      - endpoint: POST /api/v1/fleet/login\n        description: Email + password login returning a\
  \ user object and session token.\n      - ui: /profile (\"My account\" > Get API token)\n        description: Required for SSO/MFA users; API login is disabled for them.\n    sources: [docs]\n  - name: apiOnlyUserToken\n    type: http\n    scheme: bearer\n    in: header\n    header: Authorization\n    description: >-\n      Non-expiring token issued to an API-only user (fleetctl user create\n      --api-only) for automation and GitOps workflows.\n    sources: [docs]\nidentity:\n  sso: true\n  sso_protocols: [saml, oidc]\n  mfa: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fleet/refs/heads/main/authentication/fleet-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Developer Tools
- Device Management
- MDM
- Endpoint Security
- Vulnerability Management
- osquery
- Open Source
- DevOps
---

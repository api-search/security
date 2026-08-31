---
api_key_in: []
api_specs:
- filename: soothe-help-center-mirror-openapi.json
  format: json
  label: Soothe Help Center Mirror
  slug: soothe-help-center-mirror
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soothe/refs/heads/main/openapi/soothe-help-center-mirror-openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Soothe Authentication
name_suffix: Authentication
oauth_flows: []
overview: Soothe declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Soothe
provider_slug: soothe
scheme_count: 0
schemes: []
slug: soothe-authentication
source_filename: soothe-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: probed\nsource: >-\n  openapi/soothe-help-center-mirror-openapi.json (no securitySchemes) plus live probes of\n  https://api.soothe.com/ and https://www.soothe.com/sign_on/\nsummary:\n  types: []\n  api_key_in: []\n  oauth2_flows: []\nschemes: []\nnote: >-\n  Soothe publishes no authenticated API contract. The only machine-readable spec it\n  serves — the help-centre mirror schema — declares no components.securitySchemes and no\n  security requirement on any operation; that surface is anonymous read-only content.\n  The company's actual API host, api.soothe.com, is not anonymous: every request 301s to\n  /users/sign_in and returns a Rails/Devise session login form (page title \"Api | Log\n  In\") carrying a CSRF token. That is a browser session login, not a documented API\n  credential scheme, and no key type, header, scope model or token endpoint is published\n  anywhere on soothe.com. Recorded as an honest absence rather than guessed.\nobserved:\n\
  - host: https://api.soothe.com\n  status: 301\n  redirect: https://api.soothe.com/users/sign_in\n  mechanism: rails-devise-session-login\n  evidence: 'HTML form with authenticity_token; <title>Api | Log In </title>'\n  documented: false\n- host: https://www.soothe.com/sign_on/\n  status: 200\n  mechanism: consumer-account-login\n  documented: false\n- host: https://help.soothe.com\n  status: 200\n  mechanism: none\n  note: anonymous, unauthenticated read-only content service\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/soothe/refs/heads/main/authentication/soothe-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Wellness
- Health and Wellness
- Massage
- Marketplace
- On-Demand Services
- Beauty
- Corporate Wellness
- Hospitality
- Consumer Services
- Local Services
- Booking
---

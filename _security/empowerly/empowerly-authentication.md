---
api_key_in: []
api_specs:
- filename: empowerly-status-api-openapi.yml
  format: yaml
  label: Empowerly Status API
  slug: empowerly-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/empowerly/refs/heads/main/openapi/empowerly-status-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: derived
name: Empowerly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Empowerly declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Empowerly
provider_slug: empowerly
scheme_count: 0
schemes: []
slug: empowerly-authentication
source_filename: empowerly-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: derived\nsource: >-\n  openapi/empowerly-status-api-openapi.yml (no securitySchemes; global `security: []`), plus live\n  unauthenticated probes of status.empowerly.com, api.empowerly.com and app.empowerly.com 2026-08-12\nsummary: >-\n  Empowerly documents no authentication for developers because it exposes no developer API. The one\n  callable public surface is entirely unauthenticated. A separate production API host exists behind\n  the web portal and is presumed session/token authenticated, but nothing about its scheme is\n  published and none was inferred.\napis:\n- api: Empowerly Status API\n  baseURL: https://status.empowerly.com/api/v2\n  schemes: []\n  anonymous: true\n  note: >-\n    No securityScheme is declared and none is required. All eight probed endpoints returned 200 to\n    an anonymous GET with no credential of any kind. Access-Control-Allow-Origin is `*`, so the API\n    is callable directly from a browser. This is the Atlassian\
  \ Statuspage default posture, not an\n    Empowerly design decision.\n  evidence:\n  - url: https://status.empowerly.com/api/v2/summary.json\n    http_status: 200\n    credential_sent: none\nundocumented:\n- host: https://api.empowerly.com\n  scheme: unknown\n  note: >-\n    Live production API host for the student/counselor portal. No auth scheme is published, no\n    /.well-known/oauth-authorization-server (403), no /.well-known/openid-configuration, and no\n    documented token, API key or OAuth flow anywhere on empowerly.com. Only the unauthenticated\n    /health endpoint (200) responds; every other probed path 404s. Recorded as unknown — NOT guessed.\n- host: https://app.empowerly.com\n  scheme: unknown\n  note: >-\n    Student and counselor web portal (CloudFront-served SPA). Sign-in is a human web login; no\n    programmatic auth is documented and no OIDC discovery document is served.\noauth:\n  supported: false\n  discovery_probed:\n  - url: https://empowerly.com/.well-known/oauth-authorization-server\n\
  \    http_status: 404\n  - url: https://empowerly.com/.well-known/openid-configuration\n    http_status: 404\n  - url: https://api.empowerly.com/.well-known/oauth-authorization-server\n    http_status: 403\nscopes:\n  published: false\n  note: >-\n    derive-oauth-scopes.py found zero oauth2 securitySchemes across the repo, and no scopes or\n    permissions reference exists on empowerly.com. No scopes/ artifact was written.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/empowerly/refs/heads/main/authentication/empowerly-authentication.yml
summary_line: 0 schemes
tags:
- Company
- education
- edtech
- college-admissions
- counseling
- students
- career-services
- consumer-services
- status-page
---

---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: probed
name: Certificial Authentication
name_suffix: Authentication
oauth_flows: []
overview: Certificial secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Certificial
provider_slug: certificial
scheme_count: 1
schemes:
- confidence: medium
  description: 'Observed challenge scheme. The API root returns `WWW-Authenticate: Token`, indicating an opaque API token presented as `Authorization: Token <key>` (Django REST Framework TokenAuthentication). The exact token issuance flow is not publicly documented.'
  in: header
  name: TokenAuth
  parameter_name: Authorization
  scheme: Token
  sources:
  - probe:https://my.certificial.com/api/
  type: http
slug: certificial-authentication
source_filename: certificial-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: https://my.certificial.com/api/\ndocs: null\nnote: >-\n  Certificial publishes no public authentication documentation and no OpenAPI\n  definition, so this profile is not derived from a spec — it is recorded from a\n  live, anonymous probe of the platform API root. The API root answers HTTP 401\n  with an RFC 7235 WWW-Authenticate challenge naming the \"Token\" scheme and a\n  JSON body, which is the Django REST Framework TokenAuthentication signature.\n  Credentials are issued through a sales / reseller conversation, not self-serve.\nsummary:\n  types:\n  - http\n  api_key_in: []\n  oauth2_flows: []\n  self_service_credentials: false\n  public_docs: false\nschemes:\n- name: TokenAuth\n  type: http\n  scheme: Token\n  in: header\n  parameter_name: Authorization\n  description: >-\n    Observed challenge scheme. The API root returns `WWW-Authenticate: Token`,\n    indicating an opaque API token presented as `Authorization: Token\
  \ <key>`\n    (Django REST Framework TokenAuthentication). The exact token issuance flow\n    is not publicly documented.\n  confidence: medium\n  sources:\n  - probe:https://my.certificial.com/api/\nnegative_findings:\n- probe: https://my.certificial.com/.well-known/openid-configuration\n  result: soft-404\n  note: >-\n    Returns HTTP 200 but serves the single-page-app HTML shell (8403 bytes,\n    text/html) — byte-identical to a nonsense control path. Not an OIDC document.\n- probe: https://my.certificial.com/.well-known/oauth-authorization-server\n  result: soft-404\n  note: Same SPA catch-all shell. No RFC 8414 authorization-server metadata.\n- probe: https://my.certificial.com/api/oauth/token\n  result: 404\n  note: No OAuth token endpoint under the API prefix.\nx-evidence:\n- fetched: '2026-08-09'\n  url: https://my.certificial.com/api/\n  http_status: 401\n  content_type: application/json\n  www_authenticate: Token\n  allow: GET, HEAD, OPTIONS\n  body: '{\"detail\":\"Authentication\
  \ credentials were not provided.\"}'\n- fetched: '2026-08-09'\n  url: https://www.certificial.com/insurance-tracking-api\n  http_status: 200\n  note: >-\n    Product page for the Insurance Tracking API. Carries no authentication\n    documentation; the only call to action is \"Setup a Call to Discuss our API\".\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/certificial/refs/heads/main/authentication/certificial-authentication.yml
summary_line: http · 1 scheme
tags:
- Insurance
- Insurtech
- Certificate of Insurance
- Risk Management
- Compliance
- Supplier Management
- Insurance Verification
- ACORD
- Company
---

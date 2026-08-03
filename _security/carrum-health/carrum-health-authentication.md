---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: probed
name: Carrum Health Authentication
name_suffix: Authentication
oauth_flows: []
overview: Carrum Health secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Carrum Health
provider_slug: carrum-health
scheme_count: 1
schemes:
- applies_to: /api-docs
  description: 'Every platform service gates its API documentation surface behind HTTP Basic authentication. Observed response: 401 with `WWW-Authenticate: Basic realm=""`.'
  name: apiDocsBasic
  scheme: basic
  sources:
  - https://core-service.carrumhealth.com/api-docs
  - https://care-service.carrumhealth.com/api-docs
  - https://message-service.carrumhealth.com/api-docs
  - https://price-service.carrumhealth.com/api-docs
  - https://upload-service.carrumhealth.com/api-docs
  type: http
slug: carrum-health-authentication
source_filename: carrum-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live HTTP probe of the Carrum Health platform service hosts\ndocs: null\nnotes: >-\n  Carrum Health publishes no OpenAPI definition and no public authentication documentation,\n  so this profile could not be derived from a specification. It records what was actually\n  observed on the wire against the five internet-facing platform services discovered in the\n  provider's public member-application bundle. Nothing here is asserted beyond an observed\n  HTTP response.\nsummary:\n  types:\n  - http\n  api_key_in: []\n  oauth2_flows: []\n  public_developer_auth: false\n  self_service_onboarding: false\nschemes:\n- name: apiDocsBasic\n  type: http\n  scheme: basic\n  applies_to: /api-docs\n  description: >-\n    Every platform service gates its API documentation surface behind HTTP Basic\n    authentication. Observed response: 401 with `WWW-Authenticate: Basic realm=\"\"`.\n  sources:\n  - https://core-service.carrumhealth.com/api-docs\n\
  \  - https://care-service.carrumhealth.com/api-docs\n  - https://message-service.carrumhealth.com/api-docs\n  - https://price-service.carrumhealth.com/api-docs\n  - https://upload-service.carrumhealth.com/api-docs\ndiscovery:\n  openid_configuration: absent\n  oauth_authorization_server: absent\n  oauth_protected_resource: absent\n  notes: >-\n    /.well-known/openid-configuration and /.well-known/oauth-protected-resource return 404 on\n    every host; /.well-known/oauth-authorization-server returns 403 on core-service (edge\n    block, not a document). Member sign-in happens in the my.carrumhealth.com application\n    behind an activation/registration flow; the token exchange is not publicly documented.\nx-evidence:\n  fetched: '2026-08-01'\n  probes:\n  - url: https://core-service.carrumhealth.com/api-docs\n    http_status: 401\n    www_authenticate: Basic realm=\"\"\n    server_headers_observed:\n    - x-request-id\n    - x-runtime\n  - url: https://care-service.carrumhealth.com/api-docs\n\
  \    http_status: 401\n  - url: https://message-service.carrumhealth.com/api-docs\n    http_status: 401\n  - url: https://price-service.carrumhealth.com/api-docs\n    http_status: 401\n  - url: https://upload-service.carrumhealth.com/api-docs\n    http_status: 401\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carrum-health/refs/heads/main/authentication/carrum-health-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Healthcare
- Health Benefits
- Centers of Excellence
- Value-Based Care
- Bundled Payments
- Employee Benefits
- Surgery
- Care Navigation
- Digital Health
---

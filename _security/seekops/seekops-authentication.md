---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Seekops Authentication
name_suffix: Authentication
oauth_flows: []
overview: SeekOps declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: SeekOps
provider_slug: seekops
scheme_count: 0
schemes: []
slug: seekops-authentication
source_filename: seekops-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: unauthenticated HTTP probes of celsius.seekops.com, docs.seekops.com and fastr.seekops.com\nnote: >-\n  SeekOps publishes NO authentication documentation. Nothing below is derived from a\n  securityScheme or a docs page — every line is an observation from an unauthenticated\n  request. No `type: Authentication` pointer is wired at the repo level, because the\n  scoring check reads \"the provider documents authentication\" and SeekOps does not.\n  The per-API pointer records the observed posture for a reader, not a published one.\nsurfaces:\n- name: Celsius Platform API\n  host: celsius.seekops.com\n  base: https://celsius.seekops.com/api/\n  stack: Django REST Framework (inferred from the error envelope)\n  auth_required: true\n  scheme: unknown\n  evidence:\n  - url: https://celsius.seekops.com/api/\n    status: 401\n    body: '{\"detail\":\"Authentication credentials were not provided.\"}'\n    content_type: application/json\n\
  \  - url: https://celsius.seekops.com/api/users/\n    status: 401\n    body: '{\"detail\":\"Authentication credentials were not provided.\"}'\n  - url: https://celsius.seekops.com/api/sites/\n    status: 401\n    body: '{\"detail\":\"Authentication credentials were not provided.\"}'\n  note: >-\n    The 401 body is Django REST Framework's default NotAuthenticated detail string. No\n    WWW-Authenticate challenge names a scheme, so whether this is session, token, JWT or\n    key auth cannot be determined anonymously. The Celsius web front end is a separate\n    Next.js application served from the same host root.\n  schema_endpoints_probed:\n  - path: /api/schema/\n    status: 404\n  - path: /api/schema/swagger-ui/\n    status: 404\n  - path: /api/schema/redoc/\n    status: 404\n  - path: /api/docs/\n    status: 404\n  - path: /api/openapi.json\n    status: 404\n  - path: /api/v1/openapi.json\n    status: 404\n  schema_available: false\n- name: SeekOps documentation portal\n  host: docs.seekops.com\n\
  \  auth_required: true\n  scheme: openid-connect\n  provider: Microsoft Entra ID\n  evidence:\n  - url: https://docs.seekops.com/\n    status: 200\n    redirects_to: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    detail: 'response_type=code+id_token, scope=openid profile email, client_id=d414ee2d-73e5-4e5b-bb16-03ef55fea597, hosted on identity.6.azurestaticapps.net'\n  note: The documentation host exists but no page is readable without a SeekOps-issued account.\n- name: FASTR real-time telemetry\n  host: fastr.seekops.com\n  auth_required: true\n  scheme: openid-connect\n  provider: Microsoft Entra ID\n  evidence:\n  - url: https://fastr.seekops.com/\n    status: 200\n    detail: Azure Static Web Apps auth wall returning the Microsoft sign-in page for every path, including nonexistent ones.\nsummary:\n  publicly_documented: false\n  anonymous_schema_available: false\n  api_keys_self_serve: false\n  oauth_metadata_published: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/seekops/refs/heads/main/authentication/seekops-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Energy
- Oil and Gas
- Emissions
- Methane
- Environmental Monitoring
- Sensors
- Drones
- Remote Sensing
- Climate
- ESG
- Sustainability
- Analytics
- Measurement
---

---
api_key_in: []
auth_types:
- session
- unknown
description: ''
kind: authentication
layout: security
method: probed
name: Ecorobotix Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ecorobotix secures its APIs with session and unknown across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Ecorobotix
provider_slug: ecorobotix
scheme_count: 0
schemes: []
slug: ecorobotix-authentication
source_filename: ecorobotix-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: https://portal.ecorobotix.cloud/api/schema/\nnote: >-\n  Ecorobotix publishes no OpenAPI document that can be read anonymously, so this\n  profile is NOT derived from a spec. It is recorded from the observed behaviour\n  of the live portal API. derive-authentication.py found zero spec files in this\n  repo, which is correct: the schema exists but is auth-gated.\nsummary:\n  types:\n  - session\n  - unknown\n  api_key_in: []\n  oauth2_flows: []\n  public_developer_program: false\n  self_service_signup: false\nobserved:\n- surface: https://portal.ecorobotix.cloud/api/schema/\n  http_status: 401\n  content_type: application/json\n  www_authenticate: null\n  body: '{\"detail\": \"Authentication credentials were not provided.\"}'\n  server: gunicorn\n  note: >-\n    Verbatim Django REST Framework NotAuthenticated response. Confirms the API is\n    a DRF application with a drf-spectacular schema endpoint and that no\n    anonymous\
  \ access is permitted. DRF returns this message for both session and\n    token authentication classes, so the accepted credential type cannot be\n    determined without an account.\n- surface: https://portal.ecorobotix.cloud/api/schema/swagger-ui/\n  http_status: 401\n  content_type: application/json\n  note: Swagger UI is deployed but gated behind the same authentication class.\n- surface: https://portal.ecorobotix.cloud/api/\n  http_status: 302\n  redirects_to: https://portal.ecorobotix.cloud/auth/login/\n  note: >-\n    Browser-facing API paths redirect to the portal login form rather than\n    returning 401, indicating SessionAuthentication is in the DEFAULT\n    AUTHENTICATION_CLASSES list.\n- surface: https://api.ecorobotix.cloud/\n  http_status: 503\n  content_type: application/json\n  body: '{\"message\":\"Service Unavailable\"}'\n  note: >-\n    Separate AWS API Gateway host. Returns the same 503 for every path probed,\n    so no authentication scheme could be observed.\nschemes:\
  \ []\ngaps:\n- No public authentication documentation page.\n- No documented API key issuance, OAuth client registration or token endpoint.\n- No /.well-known/oauth-authorization-server or /.well-known/openid-configuration\n  on any host.\n- Credential type (session cookie vs DRF token vs JWT) is not publicly stated and\n  cannot be determined anonymously.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ecorobotix/refs/heads/main/authentication/ecorobotix-authentication.yml
summary_line: session/unknown · 0 schemes
tags:
- Company
- Agriculture
- AgTech
- Precision Agriculture
- Robotics
- Artificial Intelligence
- Computer Vision
- Machine Learning
- Sustainability
- Farm Equipment
- Switzerland
- IoT
---

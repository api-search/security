---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Heartflow Authentication
name_suffix: Authentication
oauth_flows: []
overview: HeartFlow declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: HeartFlow
provider_slug: heartflow
scheme_count: 0
schemes: []
slug: heartflow-authentication
source_filename: heartflow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: live HTTP probes of https://api.heartflow.net on 2026-08-22\nnote: >-\n  Heartflow documents no authentication publicly. Everything below was observed from the\n  API's anonymous responses, not read from a specification or a docs page, so it records\n  that the API is authenticated and what framework serves it — not how to authenticate.\n  NO `Authentication` pointer is emitted in apis.yml, because emitting one would credit\n  Heartflow with documented authentication it does not publish.\ndocumented_publicly: false\ndocs: null\ndocs_gate: >-\n  https://docs.heartflow.net/ returns 403\n  <Error><Code>MissingKey</Code><Message>Missing Key-Pair-Id query parameter or cookie\n  value</Message></Error> — a CloudFront signed-cookie gate, so the auth reference is\n  customer-only.\nobserved:\n  framework: Django REST Framework\n  framework_evidence: >-\n    Every authenticated route returns the exact DRF body\n    {\"detail\":\"Authentication\
  \ credentials were not provided.\"} with HTTP 403, and the\n    DRF browsable-schema routes /swagger/ and /redoc/ are mounted (403 rather than 404).\n  challenge_status: 403\n  www_authenticate_header: null\n  scheme: unknown\n  scheme_note: >-\n    DRF returns 403 without a WWW-Authenticate header when it cannot resolve a\n    credential, which is consistent with session or token authentication rather than\n    HTTP Basic. The concrete scheme cannot be established anonymously and is NOT guessed\n    here.\nprobes:\n- url: https://api.heartflow.net/\n  status: 403\n  body: '{\"detail\":\"Authentication credentials were not provided.\"}'\n- url: https://api.heartflow.net/api/v1/\n  status: 403\n  body: '{\"detail\":\"Authentication credentials were not provided.\"}'\n- url: https://api.heartflow.net/swagger/\n  status: 403\n- url: https://api.heartflow.net/redoc/\n  status: 403\n- url: https://api.heartflow.net/.well-known/openid-configuration\n  status: 404\n- url: https://api.heartflow.net/.well-known/oauth-authorization-server\n\
  \  status: 404\n- url: https://api.heartflow.net/.well-known/oauth-protected-resource\n  status: 404\nsecurity_schemes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/heartflow/refs/heads/main/authentication/heartflow-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Healthcare
- Medical Imaging
- Artificial Intelligence
- Cardiology
- Diagnostics
- Medical Devices
- Radiology
- Clinical Decision Support
- Machine Learning
---

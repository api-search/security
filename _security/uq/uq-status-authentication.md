---
api_key_in: []
api_specs:
- filename: uq-status-openapi.yml
  format: yaml
  label: UQ Status API
  slug: status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uq/refs/heads/main/openapi/uq-status-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Uq Status Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Queensland declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: University of Queensland
provider_slug: uq
scheme_count: 0
schemes: []
slug: uq-status-authentication
source_filename: uq-status-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "authentication: '0.1'\ngenerated: '2026-08-30'\nmethod: probed\nsource: https://status.its.uq.edu.au/index.json\nx-operator: institution\napis:\n  - name: UQ Status API\n    base_url: https://status.its.uq.edu.au\n    schemes:\n      - type: none\n        required: false\n        description: >-\n          No authentication of any kind. All five documented endpoints returned HTTP 200 to an\n          anonymous, keyless GET on 2026-08-30 with no cookie, header or token. There is no\n          registration, no API key, no OAuth flow and no rate-limit header in the response.\n    evidence:\n      - url: https://status.its.uq.edu.au/index.json\n        status: 200\n        note: keyless GET, application/json, 86,448 bytes\n      - url: https://status.its.uq.edu.au/issues/index.json\n        status: 200\n        note: keyless GET, 36,667 bytes\n      - url: https://status.its.uq.edu.au/issues/19999/index.json\n        status: 200\n        note: keyless GET, 360 bytes\nnotes:\n \
  \ - >-\n    Every other UQ surface reviewed in this run is the opposite of this one. api.library.uq.edu.au\n    returns HTTP 403 \"Request blocked\" from CloudFront to any outside client; data.uq.edu.au\n    301-redirects to uq.sharepoint.com behind Microsoft Entra sign-in; programs-courses.uq.edu.au\n    answers GET with HTTP 405 and x-amzn-waf-action: captcha. None of those are open surfaces and\n    none carry a published authentication scheme.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uq/refs/heads/main/authentication/uq-status-authentication.yml
summary_line: 0 schemes
tags:
- University
- Higher Education
- Education
- Australia
- Group of Eight
- Research
- Institutional Repository
- Identity Federation
- Status
- Library
- Research Computing
- Open Data
---

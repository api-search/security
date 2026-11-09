---
anonymous_access: false
api_key_in: []
api_specs:
- filename: arpi-ai-authentication-api-openapi.yml
  format: yaml
  label: ARPI Inc. Authentication API
  slug: arpi-ai-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arpi-ai/openapi/arpi-ai-authentication-api-openapi.yml
- filename: arpi-ai-diag-api-openapi.yml
  format: yaml
  label: ARPI Inc. Diag API
  slug: arpi-ai-diag-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arpi-ai/openapi/arpi-ai-diag-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Arpi Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: ARPI Inc. declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: ARPI Inc.
provider_slug: arpi-ai
scheme_count: 1
schemes:
- flow: clientCredentials
  scopes: {}
  tokenUrl: https://openapi.arpi.ai/api/v1/hospital/login
  type: oauth2
slug: arpi-ai-authentication
source_filename: arpi-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: searched\nsource: https://docs.arpi.ai/\nschemes:\n  - type: oauth2\n    flow: clientCredentials\n    tokenUrl: https://openapi.arpi.ai/api/v1/hospital/login\n    scopes: {}\n"
source_yaml_url: https://artifacts.apis.io/arpi-ai/authentication/arpi-ai-authentication.yml
summary_line: 1 scheme
tags:
- Medical AI
- Healthcare
- ECG
- Diagnostics
- Artificial Intelligence
---

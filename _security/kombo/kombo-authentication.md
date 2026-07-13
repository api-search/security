---
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: Kombo Unified API
  slug: unified-api
  spec_type: OpenAPI
  url: https://api.kombo.dev/openapi.json
- filename: openapi.json
  format: json
  label: Kombo Unified HRIS API
  slug: hris-api
  spec_type: OpenAPI
  url: https://api.kombo.dev/openapi.json
- filename: openapi.json
  format: json
  label: Kombo Unified ATS API
  slug: ats-api
  spec_type: OpenAPI
  url: https://api.kombo.dev/openapi.json
- filename: openapi.json
  format: json
  label: Kombo Unified ATS-Assessment API
  slug: ats-assessment-api
  spec_type: OpenAPI
  url: https://api.kombo.dev/openapi.json
- filename: openapi.json
  format: json
  label: Kombo Unified LMS API
  slug: lms-api
  spec_type: OpenAPI
  url: https://api.kombo.dev/openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Kombo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kombo secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Kombo
provider_slug: kombo
scheme_count: 1
schemes:
- description: Create an API key on the [Secrets](https://app.kombo.dev/secrets) page in the Kombo dashboard.
  name: ApiKey
  scheme: bearer
  sources:
  - openapi/kombo-openapi.json
  type: http
slug: kombo-authentication
source_filename: kombo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/kombo-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: ApiKey\n  type: http\n  scheme: bearer\n  description: Create an API key on the [Secrets](https://app.kombo.dev/secrets) page in the\n    Kombo dashboard.\n  sources:\n  - openapi/kombo-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kombo/refs/heads/main/authentication/kombo-authentication.yml
summary_line: http · 1 scheme
tags:
- ATS
- Embedded iPaaS
- HRIS
- LMS
- Payroll
- Unified API
---

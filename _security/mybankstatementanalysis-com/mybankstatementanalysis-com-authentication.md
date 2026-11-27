---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mybankstatementanalysis-com-analyses-api-openapi.yml
  format: yaml
  label: Bank Statement Analyzer Analyses API
  slug: mybankstatementanalysis-com-analyses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mybankstatementanalysis-com/openapi/mybankstatementanalysis-com-analyses-api-openapi.yml
- filename: mybankstatementanalysis-com-me-api-openapi.yml
  format: yaml
  label: Bank Statement Analyzer Me API
  slug: mybankstatementanalysis-com-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mybankstatementanalysis-com/openapi/mybankstatementanalysis-com-me-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Bank Statement Analyzer Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bank Statement Analyzer secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bank Statement Analyzer
provider_slug: mybankstatementanalysis-com
scheme_count: 1
schemes:
- description: An API key created in account settings, prefixed `mbsa_`.
  name: apiKey
  scheme: bearer
  sources:
  - openapi/api-v1-openapi.json
  type: http
slug: mybankstatementanalysis-com-authentication
source_filename: mybankstatementanalysis-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: derived\nsource: openapi/api-v1-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  description: An API key created in account settings, prefixed `mbsa_`.\n  sources:\n  - openapi/api-v1-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/mybankstatementanalysis-com/authentication/mybankstatementanalysis-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Bank Statement Analysis
- Landlords
---

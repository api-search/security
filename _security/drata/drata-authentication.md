---
api_key_in: []
api_specs:
- filename: drata-assets-api-openapi.yml
  format: yaml
  label: Drata Assets API
  slug: drata-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drata/refs/heads/main/openapi/drata-assets-api-openapi.yml
- filename: drata-audits-api-openapi.yml
  format: yaml
  label: Drata Audits API
  slug: drata-audits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drata/refs/heads/main/openapi/drata-audits-api-openapi.yml
- filename: drata-controls-api-openapi.yml
  format: yaml
  label: Drata Controls API
  slug: drata-controls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drata/refs/heads/main/openapi/drata-controls-api-openapi.yml
- filename: drata-evidence-library-api-openapi.yml
  format: yaml
  label: Drata Evidence Library API
  slug: drata-evidence-library-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drata/refs/heads/main/openapi/drata-evidence-library-api-openapi.yml
- filename: drata-frameworks-api-openapi.yml
  format: yaml
  label: Drata Frameworks API
  slug: drata-frameworks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drata/refs/heads/main/openapi/drata-frameworks-api-openapi.yml
- filename: drata-monitoring-tests-api-openapi.yml
  format: yaml
  label: Drata Monitoring Tests API
  slug: drata-monitoring-tests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drata/refs/heads/main/openapi/drata-monitoring-tests-api-openapi.yml
- filename: drata-personnel-api-openapi.yml
  format: yaml
  label: Drata Personnel API
  slug: drata-personnel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drata/refs/heads/main/openapi/drata-personnel-api-openapi.yml
- filename: drata-policies-api-openapi.yml
  format: yaml
  label: Drata Policies API
  slug: drata-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drata/refs/heads/main/openapi/drata-policies-api-openapi.yml
- filename: drata-risks-api-openapi.yml
  format: yaml
  label: Drata Risks API
  slug: drata-risks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drata/refs/heads/main/openapi/drata-risks-api-openapi.yml
- filename: drata-tasks-api-openapi.yml
  format: yaml
  label: Drata Tasks API
  slug: drata-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drata/refs/heads/main/openapi/drata-tasks-api-openapi.yml
- filename: drata-vendors-api-openapi.yml
  format: yaml
  label: Drata Vendors API
  slug: drata-vendors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drata/refs/heads/main/openapi/drata-vendors-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Drata Authentication
name_suffix: Authentication
oauth_flows: []
overview: Drata secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Drata
provider_slug: drata
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/drata-openapi.yml
  type: http
slug: drata-authentication
source_filename: drata-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/drata-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/drata-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/drata/refs/heads/main/authentication/drata-authentication.yml
summary_line: http · 1 scheme
tags:
- GRC
- Compliance
- SOC 2
- ISO 27001
- Security
---

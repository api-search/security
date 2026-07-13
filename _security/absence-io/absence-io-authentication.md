---
api_key_in: []
api_specs:
- filename: absence-io-openapi.yml
  format: yaml
  label: Absence.io API
  slug: absence-io
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/absence-io/refs/heads/main/openapi/absence-io-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Absence Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Absence.io secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Absence.io
provider_slug: absence-io
scheme_count: 1
schemes:
- description: Hawk authentication using an API key ID and API key. Generate your API key from your absence.io account profile under the Integrations tab. Use the @hapi/hawk library to generate the Authorization header with SHA256 algorithm.
  name: HawkAuth
  scheme: hawk
  sources:
  - openapi/absence-io-openapi.yml
  type: http
slug: absence-io-authentication
source_filename: absence-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/absence-io-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: HawkAuth\n  type: http\n  scheme: hawk\n  description: Hawk authentication using an API key ID and API key. Generate your API key from\n    your absence.io account profile under the Integrations tab. Use the @hapi/hawk library to\n    generate the Authorization header with SHA256 algorithm.\n  sources:\n  - openapi/absence-io-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/absence-io/refs/heads/main/authentication/absence-io-authentication.yml
summary_line: http · 1 scheme
tags:
- Absences
- Employees
- Leave Management
- HR
---

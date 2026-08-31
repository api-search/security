---
api_key_in: []
api_specs:
- filename: split-admin-api-openapi.yml
  format: yaml
  label: Split Admin API
  slug: split-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/split/refs/heads/main/openapi/split-admin-api-openapi.yml
- filename: split-evaluation-api-openapi.yml
  format: yaml
  label: Split Evaluation API
  slug: split-evaluation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/split/refs/heads/main/openapi/split-evaluation-api-openapi.yml
- filename: split-events-api-openapi.yml
  format: yaml
  label: Split Events API
  slug: split-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/split/refs/heads/main/openapi/split-events-api-openapi.yml
- filename: split-feature-flag-definitions-api-openapi.yml
  format: yaml
  label: Split Feature Flag Definitions API
  slug: split-feature-flag-definitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/split/refs/heads/main/openapi/split-feature-flag-definitions-api-openapi.yml
- filename: split-feature-flags-api-openapi.yml
  format: yaml
  label: Split Feature Flags API
  slug: split-feature-flags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/split/refs/heads/main/openapi/split-feature-flags-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Split Authentication
name_suffix: Authentication
oauth_flows: []
overview: Split secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Split
provider_slug: split
scheme_count: 1
schemes:
- description: Admin API key passed as a Bearer token in the Authorization header.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/split-admin-api-openapi.yml
  - openapi/split-feature-flag-api-openapi.yml
  type: http
slug: split-authentication
source_filename: split-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/split-admin-api-openapi.yml, openapi/split-feature-flag-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Admin API key passed as a Bearer token in the Authorization header.\n  sources:\n  - openapi/split-admin-api-openapi.yml\n  - openapi/split-feature-flag-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/split/refs/heads/main/authentication/split-authentication.yml
summary_line: http · 1 scheme
tags:
- Experimentation
- Feature Flags
- Feature Management
- Rollouts
- SDK
---

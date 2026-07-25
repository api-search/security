---
api_key_in: []
api_specs:
- filename: dryad-datasets-api-openapi.yml
  format: yaml
  label: Dryad datasets API
  slug: dryad-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dryad/refs/heads/main/openapi/dryad-datasets-api-openapi.yml
- filename: dryad-files-api-openapi.yml
  format: yaml
  label: Dryad files API
  slug: dryad-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dryad/refs/heads/main/openapi/dryad-files-api-openapi.yml
- filename: dryad-internal-api-openapi.yml
  format: yaml
  label: Dryad internal API
  slug: dryad-internal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dryad/refs/heads/main/openapi/dryad-internal-api-openapi.yml
- filename: dryad-reports-api-openapi.yml
  format: yaml
  label: Dryad reports API
  slug: dryad-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dryad/refs/heads/main/openapi/dryad-reports-api-openapi.yml
- filename: dryad-root-api-openapi.yml
  format: yaml
  label: Dryad root API
  slug: dryad-root-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dryad/refs/heads/main/openapi/dryad-root-api-openapi.yml
- filename: dryad-search-api-openapi.yml
  format: yaml
  label: Dryad search API
  slug: dryad-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dryad/refs/heads/main/openapi/dryad-search-api-openapi.yml
- filename: dryad-versions-api-openapi.yml
  format: yaml
  label: Dryad versions API
  slug: dryad-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dryad/refs/heads/main/openapi/dryad-versions-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Dryad Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dryad secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Dryad
provider_slug: dryad
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/openapi.yml
  type: http
slug: dryad-authentication
source_filename: dryad-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dryad/refs/heads/main/authentication/dryad-authentication.yml
summary_line: http · 1 scheme
tags:
- Research Data
- Open Science
- Data Repository
- Datasets
- Biology
- Ecology
- Open Access
---

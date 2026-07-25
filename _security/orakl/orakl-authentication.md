---
api_key_in: []
api_specs:
- filename: orakl-commoncontent-api-openapi.yml
  format: yaml
  label: Orakl CommonContent API
  slug: orakl-commoncontent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orakl/refs/heads/main/openapi/orakl-commoncontent-api-openapi.yml
- filename: orakl-customform-api-openapi.yml
  format: yaml
  label: Orakl CustomForm API
  slug: orakl-customform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orakl/refs/heads/main/openapi/orakl-customform-api-openapi.yml
- filename: orakl-folder-api-openapi.yml
  format: yaml
  label: Orakl Folder API
  slug: orakl-folder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orakl/refs/heads/main/openapi/orakl-folder-api-openapi.yml
- filename: orakl-login-check-api-openapi.yml
  format: yaml
  label: Orakl Login Check API
  slug: orakl-login-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orakl/refs/heads/main/openapi/orakl-login-check-api-openapi.yml
- filename: orakl-nodessources-api-openapi.yml
  format: yaml
  label: Orakl NodesSources API
  slug: orakl-nodessources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orakl/refs/heads/main/openapi/orakl-nodessources-api-openapi.yml
- filename: orakl-page-api-openapi.yml
  format: yaml
  label: Orakl Page API
  slug: orakl-page-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orakl/refs/heads/main/openapi/orakl-page-api-openapi.yml
- filename: orakl-tag-api-openapi.yml
  format: yaml
  label: Orakl Tag API
  slug: orakl-tag-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orakl/refs/heads/main/openapi/orakl-tag-api-openapi.yml
- filename: orakl-translation-api-openapi.yml
  format: yaml
  label: Orakl Translation API
  slug: orakl-translation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orakl/refs/heads/main/openapi/orakl-translation-api-openapi.yml
- filename: orakl-webresponse-api-openapi.yml
  format: yaml
  label: Orakl WebResponse API
  slug: orakl-webresponse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orakl/refs/heads/main/openapi/orakl-webresponse-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Orakl Authentication
name_suffix: Authentication
oauth_flows: []
overview: Orakl secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Orakl
provider_slug: orakl
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: JWT
  scheme: bearer
  sources:
  - openapi/orakl-website-openapi-original.json
  type: http
slug: orakl-authentication
source_filename: orakl-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/orakl-website-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: JWT\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/orakl-website-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orakl/refs/heads/main/authentication/orakl-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- TechBio
- Oncology
- Drug Development
- Artificial Intelligence
- Machine Learning
- Healthcare
- Biotechnology
- Precision Medicine
- Cancer Research
- Content Management
- JSON-LD
---

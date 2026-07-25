---
api_key_in:
- header
api_specs:
- filename: opencitations-authors-api-openapi.yml
  format: yaml
  label: OpenCitations Authors API
  slug: opencitations-authors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opencitations/refs/heads/main/openapi/opencitations-authors-api-openapi.yml
- filename: opencitations-citations-api-openapi.yml
  format: yaml
  label: OpenCitations Citations API
  slug: opencitations-citations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opencitations/refs/heads/main/openapi/opencitations-citations-api-openapi.yml
- filename: opencitations-editors-api-openapi.yml
  format: yaml
  label: OpenCitations Editors API
  slug: opencitations-editors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opencitations/refs/heads/main/openapi/opencitations-editors-api-openapi.yml
- filename: opencitations-metadata-api-openapi.yml
  format: yaml
  label: OpenCitations Metadata API
  slug: opencitations-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opencitations/refs/heads/main/openapi/opencitations-metadata-api-openapi.yml
- filename: opencitations-references-api-openapi.yml
  format: yaml
  label: OpenCitations References API
  slug: opencitations-references-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opencitations/refs/heads/main/openapi/opencitations-references-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Opencitations Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenCitations secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OpenCitations
provider_slug: opencitations
scheme_count: 1
schemes:
- description: OpenCitations Access Token obtained from https://opencitations.net/accesstoken. Recommended for application/code usage to ensure stable access.
  in: header
  name: accessToken
  parameter: authorization
  sources:
  - openapi/index-api.yml
  - openapi/meta-api.yml
  type: apiKey
slug: opencitations-authentication
source_filename: opencitations-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/index-api.yml, openapi/meta-api.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: accessToken\n  type: apiKey\n  in: header\n  parameter: authorization\n  description: OpenCitations Access Token obtained from https://opencitations.net/accesstoken.\n    Recommended for application/code usage to ensure stable access.\n  sources:\n  - openapi/index-api.yml\n  - openapi/meta-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opencitations/refs/heads/main/authentication/opencitations-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Citations
- Scholarly
- Research
- Open Science
- Bibliometrics
- DOI
- Academic
---

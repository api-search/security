---
anonymous_access: false
api_key_in: []
api_specs:
- filename: als-global-preference-api-openapi.yml
  format: yaml
  label: ALS Preference API
  slug: als-global-preference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/als-global/refs/heads/main/openapi/als-global-preference-api-openapi.yml
- filename: als-global-sample-api-openapi.yml
  format: yaml
  label: ALS Sample API
  slug: als-global-sample-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/als-global/refs/heads/main/openapi/als-global-sample-api-openapi.yml
- filename: als-global-search-api-openapi.yml
  format: yaml
  label: ALS Search API
  slug: als-global-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/als-global/refs/heads/main/openapi/als-global-search-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Als Global Authentication
name_suffix: Authentication
oauth_flows: []
overview: ALS secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ALS
provider_slug: als-global
scheme_count: 1
schemes:
- description: Basic HTTP Authentication
  name: basic
  scheme: basic
  sources:
  - openapi/als-global-webtrieve-export-openapi.yml
  type: http
slug: als-global-authentication
source_filename: als-global-authentication.yml
source_heading: Authentication Profile
source_url: openapi/als-global-webtrieve-export-openapi.yml
source_yaml: "generated: '2026-10-21'\nmethod: searched\nsource: openapi/als-global-webtrieve-export-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basic\n  type: http\n  scheme: basic\n  description: Basic HTTP Authentication\n  sources:\n  - openapi/als-global-webtrieve-export-openapi.yml\ndocs: https://www.alsglobal.com/global-integration-platform\nsources:\n- openapi/als-global-webtrieve-export-openapi.yml\n- https://www.alsglobal.com/global-integration-platform\nnote: 'Webtrieve Export API uses HTTP Basic per its contract; the brochure adds \"SSL\n  encryption determined by Webtrieve 9 user account-specific encryption key.\" Global\n  Integration Platform: \"Your ALS client support team confirms your account and scope,\n  then issues API credentials.\" and \"Connections use authenticated, encrypted API\n  access scoped to your account only.\" The credential type is not published.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/als-global/refs/heads/main/authentication/als-global-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Laboratory Testing
- Environmental Testing
- Inspection
- Certification
- Geochemistry
- Food Testing
- LIMS Integration
---

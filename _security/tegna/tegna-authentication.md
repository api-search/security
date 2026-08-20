---
api_key_in: []
api_specs:
- filename: tegna-content-api-openapi.yml
  format: yaml
  label: TEGNA Content API (WordPress REST)
  slug: tegna-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tegna/refs/heads/main/openapi/tegna-content-api-openapi.yml
- filename: tegna-premion-content-api-openapi.yml
  format: yaml
  label: PREMION Content API (WordPress REST)
  slug: tegna-premion-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tegna/refs/heads/main/openapi/tegna-premion-content-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Tegna Authentication
name_suffix: Authentication
oauth_flows: []
overview: TEGNA secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: TEGNA
provider_slug: tegna
scheme_count: 1
schemes:
- description: WordPress Application Passwords (HTTP Basic). The live index advertises the authorization endpoint at https://www.tegna.com/wp-admin/authorize-application.php. Reads on public content require no credential.
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/tegna-content-api-openapi.yml
  - openapi/tegna-premion-content-api-openapi.yml
  type: http
slug: tegna-authentication
source_filename: tegna-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: derived\nsource: openapi/tegna-content-api-openapi.yml, openapi/tegna-premion-content-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: WordPress Application Passwords (HTTP Basic). The live index advertises the authorization\n    endpoint at https://www.tegna.com/wp-admin/authorize-application.php. Reads on public content\n    require no credential.\n  sources:\n  - openapi/tegna-content-api-openapi.yml\n  - openapi/tegna-premion-content-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tegna/refs/heads/main/authentication/tegna-authentication.yml
summary_line: http · 1 scheme
tags:
- Broadcasting
- Media
- Television
- Digital Advertising
- OTT
- CTV
- Local News
- content-api
- Fortune 500
---

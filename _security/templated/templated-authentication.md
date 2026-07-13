---
api_key_in: []
api_specs:
- filename: templated-openapi.yml
  format: yaml
  label: Templated Render API
  slug: render
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/templated/refs/heads/main/openapi/templated-openapi.yml
- filename: templated-openapi.yml
  format: yaml
  label: Templated Templates API
  slug: templates
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/templated/refs/heads/main/openapi/templated-openapi.yml
- filename: templated-openapi.yml
  format: yaml
  label: Templated Renders API
  slug: renders
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/templated/refs/heads/main/openapi/templated-openapi.yml
- filename: templated-openapi.yml
  format: yaml
  label: Templated Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/templated/refs/heads/main/openapi/templated-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Templated Authentication
name_suffix: Authentication
oauth_flows: []
overview: Templated secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Templated
provider_slug: templated
scheme_count: 1
schemes:
- description: The API key must be included in all requests in the Authorization header as a Bearer token. Obtain an API key from the account dashboard at app.templated.io.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/templated-openapi.yml
  type: http
slug: templated-authentication
source_filename: templated-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/templated-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: The API key must be included in all requests in the Authorization header as a\n    Bearer token. Obtain an API key from the account dashboard at app.templated.io.\n  sources:\n  - openapi/templated-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/templated/refs/heads/main/authentication/templated-authentication.yml
summary_line: http · 1 scheme
tags:
- Image Generation
- PDF Generation
- Templates
- Rendering
- Automation
---

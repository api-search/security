---
anonymous_access: false
api_key_in: []
api_specs:
- filename: pagegoat-com-free-link-claim-controller-api-openapi.yml
  format: yaml
  label: PageGoat Free Link Claim Controller API
  slug: pagegoat-com-free-link-claim-controller-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pagegoat-com/openapi/pagegoat-com-free-link-claim-controller-api-openapi.yml
- filename: pagegoat-com-me-controller-api-openapi.yml
  format: yaml
  label: PageGoat Me Controller API
  slug: pagegoat-com-me-controller-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pagegoat-com/openapi/pagegoat-com-me-controller-api-openapi.yml
- filename: pagegoat-com-project-controller-api-openapi.yml
  format: yaml
  label: PageGoat Project Controller API
  slug: pagegoat-com-project-controller-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pagegoat-com/openapi/pagegoat-com-project-controller-api-openapi.yml
- filename: pagegoat-com-site-controller-api-openapi.yml
  format: yaml
  label: PageGoat Site Controller API
  slug: pagegoat-com-site-controller-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pagegoat-com/openapi/pagegoat-com-site-controller-api-openapi.yml
- filename: pagegoat-com-usage-controller-api-openapi.yml
  format: yaml
  label: PageGoat Usage Controller API
  slug: pagegoat-com-usage-controller-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pagegoat-com/openapi/pagegoat-com-usage-controller-api-openapi.yml
- filename: pagegoat-com-workspace-controller-api-openapi.yml
  format: yaml
  label: PageGoat Workspace Controller API
  slug: pagegoat-com-workspace-controller-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pagegoat-com/openapi/pagegoat-com-workspace-controller-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: PageGoat Authentication
name_suffix: Authentication
oauth_flows: []
overview: PageGoat secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: PageGoat
provider_slug: pagegoat-com
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearer-jwt
  scheme: bearer
  sources:
  - openapi/pagegoat-com-openapi.yml
  type: http
slug: pagegoat-com-authentication
source_filename: pagegoat-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: derived\nsource: openapi/pagegoat-com-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer-jwt\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/pagegoat-com-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/pagegoat-com/authentication/pagegoat-com-authentication.yml
summary_line: http · 1 scheme
tags:
- File Sharing
- LinkGeneration
- ContentHosting
- Developer Tools
- Software-as-a-Service
---

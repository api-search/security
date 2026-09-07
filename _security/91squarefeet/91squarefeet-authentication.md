---
anonymous_access: false
api_key_in: []
api_specs:
- filename: 91squarefeet-content-api-openapi.yml
  format: yaml
  label: 91Squarefeet Content API
  slug: 91squarefeet-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/91squarefeet/refs/heads/main/openapi/91squarefeet-content-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: 91Squarefeet Authentication
name_suffix: Authentication
oauth_flows: []
overview: 91Squarefeet secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: 91Squarefeet
provider_slug: 91squarefeet
scheme_count: 1
schemes:
- description: 'WordPress Application Passwords (HTTP Basic). Required only for write operations and the authenticated namespaces, which are not described in this document. Authorization endpoint: https://91squarefeet.com/wp-admin/authorize-application.php'
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/91squarefeet-content-api-openapi.yml
  type: http
slug: 91squarefeet-authentication
source_filename: 91squarefeet-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: derived\nsource: openapi/91squarefeet-content-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: 'WordPress Application Passwords (HTTP Basic). Required only for write operations\n    and the authenticated namespaces, which are not described in this document. Authorization\n    endpoint: https://91squarefeet.com/wp-admin/authorize-application.php'\n  sources:\n  - openapi/91squarefeet-content-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/91squarefeet/refs/heads/main/authentication/91squarefeet-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Construction
- Retail
- Interior Design
- Real Estate
- Project Management
- Supply Chain
- India
- Content
- WordPress
---

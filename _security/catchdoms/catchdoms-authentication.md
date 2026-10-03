---
anonymous_access: false
api_key_in: []
api_specs:
- filename: catchdoms-domains-api-openapi.yml
  format: yaml
  label: CatchDoms Expired Domains API Domains API
  slug: catchdoms-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/catchdoms/refs/heads/main/openapi/catchdoms-domains-api-openapi.yml
- filename: catchdoms-free-api-openapi.yml
  format: yaml
  label: CatchDoms Expired Domains API Free API
  slug: catchdoms-free-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/catchdoms/refs/heads/main/openapi/catchdoms-free-api-openapi.yml
- filename: catchdoms-pending-delete-api-openapi.yml
  format: yaml
  label: CatchDoms Expired Domains API Pending Delete API
  slug: catchdoms-pending-delete-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/catchdoms/refs/heads/main/openapi/catchdoms-pending-delete-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Catchdoms Authentication
name_suffix: Authentication
oauth_flows: []
overview: CatchDoms Expired Domains API secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CatchDoms Expired Domains API
provider_slug: catchdoms
scheme_count: 1
schemes:
- description: API token from your CatchDoms account. Get one at https://catchdoms.com/api-access
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/catchdoms-openapi.yml
  type: http
slug: catchdoms-authentication
source_filename: catchdoms-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: derived\nsource: openapi/catchdoms-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: API token from your CatchDoms account. Get one at https://catchdoms.com/api-access\n  sources:\n  - openapi/catchdoms-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/catchdoms/refs/heads/main/authentication/catchdoms-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Domains
- SEO
- Expired
---

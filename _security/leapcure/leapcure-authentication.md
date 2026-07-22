---
api_key_in: []
api_specs:
- filename: leapcure-blog-content-openapi.yml
  format: yaml
  label: Leapcure Blog Content API
  slug: leapcure-blog-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapcure/refs/heads/main/openapi/leapcure-blog-content-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Leapcure Authentication
name_suffix: Authentication
oauth_flows: []
overview: Leapcure secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Leapcure
provider_slug: leapcure
scheme_count: 1
schemes:
- description: WordPress application passwords. Authorize at https://blog.leapcure.com/wp-admin/authorize-application.php (advertised in the /wp-json/ discovery document).
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/leapcure-blog-content-openapi.yml
  type: http
slug: leapcure-authentication
source_filename: leapcure-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/leapcure-blog-content-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: WordPress application passwords. Authorize at https://blog.leapcure.com/wp-admin/authorize-application.php\n    (advertised in the /wp-json/ discovery document).\n  sources:\n  - openapi/leapcure-blog-content-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leapcure/refs/heads/main/authentication/leapcure-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Clinical Trials
- Patient Recruitment
- Healthcare
- Blog
- Content API
- WordPress
---

---
api_key_in: []
api_specs:
- filename: colossal-biosciences-content-openapi.yml
  format: yaml
  label: Colossal Biosciences Content API (WordPress REST wp/v2)
  slug: content
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/colossal-biosciences/refs/heads/main/openapi/colossal-biosciences-content-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Colossal Biosciences Authentication
name_suffix: Authentication
oauth_flows: []
overview: Colossal Biosciences secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Colossal Biosciences
provider_slug: colossal-biosciences
scheme_count: 1
schemes:
- description: WordPress Application Passwords, advertised by the site at https://colossal.com/wp-json/ under authentication.application-passwords; authorization endpoint https://colossal.com/wp-admin/authorize-application.php. Read operations on wp/v2 are anonymous.
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/colossal-biosciences-content-openapi.yml
  type: http
slug: colossal-biosciences-authentication
source_filename: colossal-biosciences-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: derived\nsource: openapi/colossal-biosciences-content-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: WordPress Application Passwords, advertised by the site at https://colossal.com/wp-json/\n    under authentication.application-passwords; authorization endpoint https://colossal.com/wp-admin/authorize-application.php.\n    Read operations on wp/v2 are anonymous.\n  sources:\n  - openapi/colossal-biosciences-content-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/colossal-biosciences/refs/heads/main/authentication/colossal-biosciences-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Biotechnology
- Genomics
- Life Sciences
- Conservation
- De-Extinction
- Synthetic Biology
- Research
- Content
---

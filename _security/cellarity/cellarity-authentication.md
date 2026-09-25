---
anonymous_access: false
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Cellarity Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cellarity secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cellarity
provider_slug: cellarity
scheme_count: 1
schemes:
- description: WordPress Application Passwords, advertised by the site at https://cellarity.com/wp-json/ under authentication.application-passwords; authorization endpoint https://cellarity.com/wp-admin/authorize-application.php. Read operations on wp/v2 are anonymous.
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/cellarity-content-openapi.yml
  type: http
slug: cellarity-authentication
source_filename: cellarity-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: derived\nsource: openapi/cellarity-content-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: WordPress Application Passwords, advertised by the site at https://cellarity.com/wp-json/\n    under authentication.application-passwords; authorization endpoint https://cellarity.com/wp-admin/authorize-application.php.\n    Read operations on wp/v2 are anonymous.\n  sources:\n  - openapi/cellarity-content-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cellarity/refs/heads/main/authentication/cellarity-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Biotechnology
- Drug Discovery
- Life Sciences
- Artificial Intelligence
- Machine Learning
- Single Cell
- Transcriptomics
- Pharmaceuticals
- Clinical Trials
- Hematology
- Research
- Content
---

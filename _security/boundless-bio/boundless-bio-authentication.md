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
name: Boundless Bio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Boundless Bio secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Boundless Bio
provider_slug: boundless-bio
scheme_count: 1
schemes:
- description: WordPress Application Passwords, advertised by the site at https://boundlessbio.com/wp-json/ under authentication.application-passwords; authorization endpoint https://boundlessbio.com/wp-admin/authorize-application.php. Read operations on wp/v2 are anonymous.
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/boundless-bio-content-openapi.yml
  type: http
slug: boundless-bio-authentication
source_filename: boundless-bio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-08'\nmethod: derived\nsource: openapi/boundless-bio-content-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: WordPress Application Passwords, advertised by the site at https://boundlessbio.com/wp-json/\n    under authentication.application-passwords; authorization endpoint https://boundlessbio.com/wp-admin/authorize-application.php.\n    Read operations on wp/v2 are anonymous.\n  sources:\n  - openapi/boundless-bio-content-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boundless-bio/refs/heads/main/authentication/boundless-bio-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Biotechnology
- Oncology
- Precision Medicine
- Drug Discovery
- Life Sciences
- Pharmaceuticals
- Clinical Trials
- Genomics
- Diagnostics
- Research
- Content
---

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
name: Kartos Therapeutics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kartos Therapeutics secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Kartos Therapeutics
provider_slug: kartos-therapeutics
scheme_count: 1
schemes:
- description: WordPress application passwords, advertised by the site's own route index at `/wp-json/` (`authentication.application-passwords.endpoints.authorization` → https://kartosthera.com/wp-admin/authorize-application.php). Application passwords are issued to existing WordPress accounts only; there is no public sign-up, no developer registration and no self-service credential issuance. Every operation mod
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/kartos-therapeutics-content-openapi.yml
  type: http
slug: kartos-therapeutics-authentication
source_filename: kartos-therapeutics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: derived\nsource: openapi/kartos-therapeutics-content-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: WordPress application passwords, advertised by the site's own route index at\n    `/wp-json/` (`authentication.application-passwords.endpoints.authorization` → https://kartosthera.com/wp-admin/authorize-application.php).\n    Application passwords are issued to existing WordPress accounts only; there is no public\n    sign-up, no developer registration and no self-service credential issuance. Every operation\n    mod\n  sources:\n  - openapi/kartos-therapeutics-content-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kartos-therapeutics/refs/heads/main/authentication/kartos-therapeutics-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Oncology
- Hematology
- Rare Disease
- Precision Medicine
- Clinical Trials
- Life Sciences
- content-api
---

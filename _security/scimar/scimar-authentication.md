---
api_key_in: []
api_specs:
- filename: scimar-content-openapi.yml
  format: yaml
  label: Scimar Content API (WordPress REST wp/v2)
  slug: content
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scimar/refs/heads/main/openapi/scimar-content-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Scimar Authentication
name_suffix: Authentication
oauth_flows: []
overview: Scimar secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Scimar
provider_slug: scimar
scheme_count: 1
schemes:
- description: WordPress Application Passwords (HTTP Basic). The scimar.ca WordPress install registers the application-passwords routes at /wp/v2/users/{user_id}/application-passwords and the authorization endpoint at https://scimar.ca/wp-admin/authorize-application.php. Read operations on wp/v2 are anonymous.
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/scimar-content-openapi.yml
  type: http
slug: scimar-authentication
source_filename: scimar-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: derived\nsource: openapi/scimar-content-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: WordPress Application Passwords (HTTP Basic). The scimar.ca WordPress install\n    registers the application-passwords routes at /wp/v2/users/{user_id}/application-passwords\n    and the authorization endpoint at https://scimar.ca/wp-admin/authorize-application.php.\n    Read operations on wp/v2 are anonymous.\n  sources:\n  - openapi/scimar-content-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scimar/refs/heads/main/authentication/scimar-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Biotechnology
- Life Sciences
- Pharmaceuticals
- Diabetes
- Diagnostics
- Clinical Trials
- Health
- Nutrition
- Research
- Canada
- Content
---

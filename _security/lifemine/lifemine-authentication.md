---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: lifemine-board-api-openapi.yml
  format: yaml
  label: LifeMine Board API
  slug: lifemine-board-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lifemine/refs/heads/main/openapi/lifemine-board-api-openapi.yml
- filename: lifemine-departments-api-openapi.yml
  format: yaml
  label: LifeMine Departments API
  slug: lifemine-departments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lifemine/refs/heads/main/openapi/lifemine-departments-api-openapi.yml
- filename: lifemine-education-api-openapi.yml
  format: yaml
  label: LifeMine Education API
  slug: lifemine-education-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lifemine/refs/heads/main/openapi/lifemine-education-api-openapi.yml
- filename: lifemine-jobs-api-openapi.yml
  format: yaml
  label: LifeMine Jobs API
  slug: lifemine-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lifemine/refs/heads/main/openapi/lifemine-jobs-api-openapi.yml
- filename: lifemine-offices-api-openapi.yml
  format: yaml
  label: LifeMine Offices API
  slug: lifemine-offices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lifemine/refs/heads/main/openapi/lifemine-offices-api-openapi.yml
- filename: lifemine-sections-api-openapi.yml
  format: yaml
  label: LifeMine Sections API
  slug: lifemine-sections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lifemine/refs/heads/main/openapi/lifemine-sections-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Lifemine Authentication
name_suffix: Authentication
oauth_flows: []
overview: LifeMine secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: LifeMine
provider_slug: lifemine
scheme_count: 2
schemes:
- description: WordPress Application Passwords (RFC 7617 Basic). Route /wp/v2/users/{user_id}/application-passwords is registered on this host. Write access only; not issued to the public.
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/lifemine-content-openapi.yml
  type: http
- description: WordPress cookie authentication with an X-WP-Nonce header (first-party browser context only). Advertised in Access-Control-Allow-Headers on this host.
  in: header
  name: cookieNonce
  parameter: X-WP-Nonce
  sources:
  - openapi/lifemine-content-openapi.yml
  type: apiKey
slug: lifemine-authentication
source_filename: lifemine-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: derived\nsource: openapi/lifemine-content-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: WordPress Application Passwords (RFC 7617 Basic). Route /wp/v2/users/{user_id}/application-passwords\n    is registered on this host. Write access only; not issued to the public.\n  sources:\n  - openapi/lifemine-content-openapi.yml\n- name: cookieNonce\n  type: apiKey\n  in: header\n  parameter: X-WP-Nonce\n  description: WordPress cookie authentication with an X-WP-Nonce header (first-party browser\n    context only). Advertised in Access-Control-Allow-Headers on this host.\n  sources:\n  - openapi/lifemine-content-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lifemine/refs/heads/main/authentication/lifemine-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Drug Discovery
- Life Sciences
- Clinical Trials
- Genomics
- Content
- Careers
- WordPress
---

---
api_key_in: []
api_specs:
- filename: scimar-comments-api-openapi.yml
  format: yaml
  label: Scimar Comments API
  slug: scimar-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scimar/refs/heads/main/openapi/scimar-comments-api-openapi.yml
- filename: scimar-discovery-api-openapi.yml
  format: yaml
  label: Scimar Discovery API
  slug: scimar-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scimar/refs/heads/main/openapi/scimar-discovery-api-openapi.yml
- filename: scimar-media-api-openapi.yml
  format: yaml
  label: Scimar Media API
  slug: scimar-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scimar/refs/heads/main/openapi/scimar-media-api-openapi.yml
- filename: scimar-pages-api-openapi.yml
  format: yaml
  label: Scimar Pages API
  slug: scimar-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scimar/refs/heads/main/openapi/scimar-pages-api-openapi.yml
- filename: scimar-posts-api-openapi.yml
  format: yaml
  label: Scimar Posts API
  slug: scimar-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scimar/refs/heads/main/openapi/scimar-posts-api-openapi.yml
- filename: scimar-search-api-openapi.yml
  format: yaml
  label: Scimar Search API
  slug: scimar-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scimar/refs/heads/main/openapi/scimar-search-api-openapi.yml
- filename: scimar-settings-api-openapi.yml
  format: yaml
  label: Scimar Settings API
  slug: scimar-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scimar/refs/heads/main/openapi/scimar-settings-api-openapi.yml
- filename: scimar-taxonomy-api-openapi.yml
  format: yaml
  label: Scimar Taxonomy API
  slug: scimar-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scimar/refs/heads/main/openapi/scimar-taxonomy-api-openapi.yml
- filename: scimar-users-api-openapi.yml
  format: yaml
  label: Scimar Users API
  slug: scimar-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scimar/refs/heads/main/openapi/scimar-users-api-openapi.yml
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

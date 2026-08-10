---
api_key_in:
- header
api_specs:
- filename: abcuro-careers-api-openapi.yml
  format: yaml
  label: Abcuro Careers API
  slug: abcuro-careers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abcuro/refs/heads/main/openapi/abcuro-careers-api-openapi.yml
- filename: abcuro-comments-api-openapi.yml
  format: yaml
  label: Abcuro Comments API
  slug: abcuro-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abcuro/refs/heads/main/openapi/abcuro-comments-api-openapi.yml
- filename: abcuro-discovery-api-openapi.yml
  format: yaml
  label: Abcuro Discovery API
  slug: abcuro-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abcuro/refs/heads/main/openapi/abcuro-discovery-api-openapi.yml
- filename: abcuro-investors-api-openapi.yml
  format: yaml
  label: Abcuro Investors API
  slug: abcuro-investors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abcuro/refs/heads/main/openapi/abcuro-investors-api-openapi.yml
- filename: abcuro-media-api-openapi.yml
  format: yaml
  label: Abcuro Media API
  slug: abcuro-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abcuro/refs/heads/main/openapi/abcuro-media-api-openapi.yml
- filename: abcuro-pages-api-openapi.yml
  format: yaml
  label: Abcuro Pages API
  slug: abcuro-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abcuro/refs/heads/main/openapi/abcuro-pages-api-openapi.yml
- filename: abcuro-people-api-openapi.yml
  format: yaml
  label: Abcuro People API
  slug: abcuro-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abcuro/refs/heads/main/openapi/abcuro-people-api-openapi.yml
- filename: abcuro-press-releases-api-openapi.yml
  format: yaml
  label: Abcuro Press Releases API
  slug: abcuro-press-releases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abcuro/refs/heads/main/openapi/abcuro-press-releases-api-openapi.yml
- filename: abcuro-publications-api-openapi.yml
  format: yaml
  label: Abcuro Publications API
  slug: abcuro-publications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abcuro/refs/heads/main/openapi/abcuro-publications-api-openapi.yml
- filename: abcuro-search-api-openapi.yml
  format: yaml
  label: Abcuro Search API
  slug: abcuro-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abcuro/refs/heads/main/openapi/abcuro-search-api-openapi.yml
- filename: abcuro-taxonomy-api-openapi.yml
  format: yaml
  label: Abcuro Taxonomy API
  slug: abcuro-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abcuro/refs/heads/main/openapi/abcuro-taxonomy-api-openapi.yml
- filename: abcuro-users-api-openapi.yml
  format: yaml
  label: Abcuro Users API
  slug: abcuro-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abcuro/refs/heads/main/openapi/abcuro-users-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Abcuro Authentication
name_suffix: Authentication
oauth_flows: []
overview: Abcuro secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Abcuro
provider_slug: abcuro
scheme_count: 2
schemes:
- description: WordPress application passwords (RFC 7617 Basic over TLS). The live route index advertises the authorization endpoint at https://abcuro.com/wp-admin/authorize-application.php. Required for every write operation and for the edit context; not available to the public.
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/abcuro-content-openapi.yml
  type: http
- description: WordPress cookie authentication paired with an X-WP-Nonce header; used by the site's own admin and block-editor UI.
  in: header
  name: cookieNonce
  parameter: X-WP-Nonce
  sources:
  - openapi/abcuro-content-openapi.yml
  type: apiKey
slug: abcuro-authentication
source_filename: abcuro-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: derived\nsource: openapi/abcuro-content-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: WordPress application passwords (RFC 7617 Basic over TLS). The live route index\n    advertises the authorization endpoint at https://abcuro.com/wp-admin/authorize-application.php.\n    Required for every write operation and for the edit context; not available to the public.\n  sources:\n  - openapi/abcuro-content-openapi.yml\n- name: cookieNonce\n  type: apiKey\n  in: header\n  parameter: X-WP-Nonce\n  description: WordPress cookie authentication paired with an X-WP-Nonce header; used by the\n    site's own admin and block-editor UI.\n  sources:\n  - openapi/abcuro-content-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abcuro/refs/heads/main/authentication/abcuro-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- biotechnology
- pharmaceuticals
- immunology
- autoimmune-disease
- oncology
- clinical-trials
- life-sciences
- drug-development
- healthcare
- content-api
- wordpress
---

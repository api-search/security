---
api_key_in: []
api_specs:
- filename: colossal-biosciences-categories-api-openapi.yml
  format: yaml
  label: Colossal Biosciences Categories API
  slug: colossal-biosciences-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/colossal-biosciences/refs/heads/main/openapi/colossal-biosciences-categories-api-openapi.yml
- filename: colossal-biosciences-comments-api-openapi.yml
  format: yaml
  label: Colossal Biosciences Comments API
  slug: colossal-biosciences-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/colossal-biosciences/refs/heads/main/openapi/colossal-biosciences-comments-api-openapi.yml
- filename: colossal-biosciences-discovery-api-openapi.yml
  format: yaml
  label: Colossal Biosciences Discovery API
  slug: colossal-biosciences-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/colossal-biosciences/refs/heads/main/openapi/colossal-biosciences-discovery-api-openapi.yml
- filename: colossal-biosciences-media-api-openapi.yml
  format: yaml
  label: Colossal Biosciences Media API
  slug: colossal-biosciences-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/colossal-biosciences/refs/heads/main/openapi/colossal-biosciences-media-api-openapi.yml
- filename: colossal-biosciences-pages-api-openapi.yml
  format: yaml
  label: Colossal Biosciences Pages API
  slug: colossal-biosciences-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/colossal-biosciences/refs/heads/main/openapi/colossal-biosciences-pages-api-openapi.yml
- filename: colossal-biosciences-posts-api-openapi.yml
  format: yaml
  label: Colossal Biosciences Posts API
  slug: colossal-biosciences-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/colossal-biosciences/refs/heads/main/openapi/colossal-biosciences-posts-api-openapi.yml
- filename: colossal-biosciences-search-api-openapi.yml
  format: yaml
  label: Colossal Biosciences Search API
  slug: colossal-biosciences-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/colossal-biosciences/refs/heads/main/openapi/colossal-biosciences-search-api-openapi.yml
- filename: colossal-biosciences-settings-api-openapi.yml
  format: yaml
  label: Colossal Biosciences Settings API
  slug: colossal-biosciences-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/colossal-biosciences/refs/heads/main/openapi/colossal-biosciences-settings-api-openapi.yml
- filename: colossal-biosciences-tags-api-openapi.yml
  format: yaml
  label: Colossal Biosciences Tags API
  slug: colossal-biosciences-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/colossal-biosciences/refs/heads/main/openapi/colossal-biosciences-tags-api-openapi.yml
- filename: colossal-biosciences-users-api-openapi.yml
  format: yaml
  label: Colossal Biosciences Users API
  slug: colossal-biosciences-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/colossal-biosciences/refs/heads/main/openapi/colossal-biosciences-users-api-openapi.yml
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

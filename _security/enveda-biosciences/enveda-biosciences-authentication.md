---
api_key_in: []
api_specs:
- filename: enveda-biosciences-comments-api-openapi.yml
  format: yaml
  label: Enveda Comments API
  slug: enveda-biosciences-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enveda-biosciences/refs/heads/main/openapi/enveda-biosciences-comments-api-openapi.yml
- filename: enveda-biosciences-discovery-api-openapi.yml
  format: yaml
  label: Enveda Discovery API
  slug: enveda-biosciences-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enveda-biosciences/refs/heads/main/openapi/enveda-biosciences-discovery-api-openapi.yml
- filename: enveda-biosciences-issues-api-openapi.yml
  format: yaml
  label: Enveda Issues API
  slug: enveda-biosciences-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enveda-biosciences/refs/heads/main/openapi/enveda-biosciences-issues-api-openapi.yml
- filename: enveda-biosciences-media-api-openapi.yml
  format: yaml
  label: Enveda Media API
  slug: enveda-biosciences-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enveda-biosciences/refs/heads/main/openapi/enveda-biosciences-media-api-openapi.yml
- filename: enveda-biosciences-news-api-openapi.yml
  format: yaml
  label: Enveda News API
  slug: enveda-biosciences-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enveda-biosciences/refs/heads/main/openapi/enveda-biosciences-news-api-openapi.yml
- filename: enveda-biosciences-pages-api-openapi.yml
  format: yaml
  label: Enveda Pages API
  slug: enveda-biosciences-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enveda-biosciences/refs/heads/main/openapi/enveda-biosciences-pages-api-openapi.yml
- filename: enveda-biosciences-people-api-openapi.yml
  format: yaml
  label: Enveda People API
  slug: enveda-biosciences-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enveda-biosciences/refs/heads/main/openapi/enveda-biosciences-people-api-openapi.yml
- filename: enveda-biosciences-posts-api-openapi.yml
  format: yaml
  label: Enveda Posts API
  slug: enveda-biosciences-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enveda-biosciences/refs/heads/main/openapi/enveda-biosciences-posts-api-openapi.yml
- filename: enveda-biosciences-search-api-openapi.yml
  format: yaml
  label: Enveda Search API
  slug: enveda-biosciences-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enveda-biosciences/refs/heads/main/openapi/enveda-biosciences-search-api-openapi.yml
- filename: enveda-biosciences-settings-api-openapi.yml
  format: yaml
  label: Enveda Settings API
  slug: enveda-biosciences-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enveda-biosciences/refs/heads/main/openapi/enveda-biosciences-settings-api-openapi.yml
- filename: enveda-biosciences-taxonomy-api-openapi.yml
  format: yaml
  label: Enveda Taxonomy API
  slug: enveda-biosciences-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enveda-biosciences/refs/heads/main/openapi/enveda-biosciences-taxonomy-api-openapi.yml
- filename: enveda-biosciences-trial-sites-api-openapi.yml
  format: yaml
  label: Enveda Trial Sites API
  slug: enveda-biosciences-trial-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enveda-biosciences/refs/heads/main/openapi/enveda-biosciences-trial-sites-api-openapi.yml
- filename: enveda-biosciences-users-api-openapi.yml
  format: yaml
  label: Enveda Users API
  slug: enveda-biosciences-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enveda-biosciences/refs/heads/main/openapi/enveda-biosciences-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Enveda Biosciences Authentication
name_suffix: Authentication
oauth_flows: []
overview: Enveda secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Enveda
provider_slug: enveda-biosciences
scheme_count: 1
schemes:
- description: WordPress Application Passwords, advertised by the site at https://enveda.com/wp-json/ under authentication.application-passwords; authorization endpoint https://enveda.com/wp-admin/authorize-application.php. Read operations on wp/v2 are anonymous.
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/enveda-biosciences-content-openapi.yml
  type: http
slug: enveda-biosciences-authentication
source_filename: enveda-biosciences-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: derived\nsource: openapi/enveda-biosciences-content-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: WordPress Application Passwords, advertised by the site at https://enveda.com/wp-json/\n    under authentication.application-passwords; authorization endpoint https://enveda.com/wp-admin/authorize-application.php.\n    Read operations on wp/v2 are anonymous.\n  sources:\n  - openapi/enveda-biosciences-content-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/enveda-biosciences/refs/heads/main/authentication/enveda-biosciences-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Biotechnology
- Drug Discovery
- Life Sciences
- Artificial Intelligence
- Machine-Learning
- Metabolomics
- Natural Products
- Pharmaceuticals
- Clinical Trials
- Research
- Content
---

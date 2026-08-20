---
api_key_in: []
api_specs:
- filename: cellarity-case-studies-api-openapi.yml
  format: yaml
  label: Cellarity Case Studies API
  slug: cellarity-case-studies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cellarity/refs/heads/main/openapi/cellarity-case-studies-api-openapi.yml
- filename: cellarity-comments-api-openapi.yml
  format: yaml
  label: Cellarity Comments API
  slug: cellarity-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cellarity/refs/heads/main/openapi/cellarity-comments-api-openapi.yml
- filename: cellarity-discovery-api-openapi.yml
  format: yaml
  label: Cellarity Discovery API
  slug: cellarity-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cellarity/refs/heads/main/openapi/cellarity-discovery-api-openapi.yml
- filename: cellarity-events-api-openapi.yml
  format: yaml
  label: Cellarity Events API
  slug: cellarity-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cellarity/refs/heads/main/openapi/cellarity-events-api-openapi.yml
- filename: cellarity-media-api-openapi.yml
  format: yaml
  label: Cellarity Media API
  slug: cellarity-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cellarity/refs/heads/main/openapi/cellarity-media-api-openapi.yml
- filename: cellarity-news-api-openapi.yml
  format: yaml
  label: Cellarity News API
  slug: cellarity-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cellarity/refs/heads/main/openapi/cellarity-news-api-openapi.yml
- filename: cellarity-pages-api-openapi.yml
  format: yaml
  label: Cellarity Pages API
  slug: cellarity-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cellarity/refs/heads/main/openapi/cellarity-pages-api-openapi.yml
- filename: cellarity-people-api-openapi.yml
  format: yaml
  label: Cellarity People API
  slug: cellarity-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cellarity/refs/heads/main/openapi/cellarity-people-api-openapi.yml
- filename: cellarity-pipeline-api-openapi.yml
  format: yaml
  label: Cellarity Pipeline API
  slug: cellarity-pipeline-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cellarity/refs/heads/main/openapi/cellarity-pipeline-api-openapi.yml
- filename: cellarity-posts-api-openapi.yml
  format: yaml
  label: Cellarity Posts API
  slug: cellarity-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cellarity/refs/heads/main/openapi/cellarity-posts-api-openapi.yml
- filename: cellarity-projects-api-openapi.yml
  format: yaml
  label: Cellarity Projects API
  slug: cellarity-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cellarity/refs/heads/main/openapi/cellarity-projects-api-openapi.yml
- filename: cellarity-search-api-openapi.yml
  format: yaml
  label: Cellarity Search API
  slug: cellarity-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cellarity/refs/heads/main/openapi/cellarity-search-api-openapi.yml
- filename: cellarity-settings-api-openapi.yml
  format: yaml
  label: Cellarity Settings API
  slug: cellarity-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cellarity/refs/heads/main/openapi/cellarity-settings-api-openapi.yml
- filename: cellarity-taxonomy-api-openapi.yml
  format: yaml
  label: Cellarity Taxonomy API
  slug: cellarity-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cellarity/refs/heads/main/openapi/cellarity-taxonomy-api-openapi.yml
- filename: cellarity-users-api-openapi.yml
  format: yaml
  label: Cellarity Users API
  slug: cellarity-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cellarity/refs/heads/main/openapi/cellarity-users-api-openapi.yml
- filename: cellarity-video-api-openapi.yml
  format: yaml
  label: Cellarity Video API
  slug: cellarity-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cellarity/refs/heads/main/openapi/cellarity-video-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
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
- Machine-Learning
- Single Cell
- Transcriptomics
- Pharmaceuticals
- Clinical Trials
- Hematology
- Research
- Content
---

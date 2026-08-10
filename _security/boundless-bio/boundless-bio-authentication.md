---
api_key_in: []
api_specs:
- filename: boundless-bio-comments-api-openapi.yml
  format: yaml
  label: Boundless Bio Comments API
  slug: boundless-bio-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boundless-bio/refs/heads/main/openapi/boundless-bio-comments-api-openapi.yml
- filename: boundless-bio-discovery-api-openapi.yml
  format: yaml
  label: Boundless Bio Discovery API
  slug: boundless-bio-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boundless-bio/refs/heads/main/openapi/boundless-bio-discovery-api-openapi.yml
- filename: boundless-bio-leadership-api-openapi.yml
  format: yaml
  label: Boundless Bio Leadership API
  slug: boundless-bio-leadership-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boundless-bio/refs/heads/main/openapi/boundless-bio-leadership-api-openapi.yml
- filename: boundless-bio-media-api-openapi.yml
  format: yaml
  label: Boundless Bio Media API
  slug: boundless-bio-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boundless-bio/refs/heads/main/openapi/boundless-bio-media-api-openapi.yml
- filename: boundless-bio-pages-api-openapi.yml
  format: yaml
  label: Boundless Bio Pages API
  slug: boundless-bio-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boundless-bio/refs/heads/main/openapi/boundless-bio-pages-api-openapi.yml
- filename: boundless-bio-posts-api-openapi.yml
  format: yaml
  label: Boundless Bio Posts API
  slug: boundless-bio-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boundless-bio/refs/heads/main/openapi/boundless-bio-posts-api-openapi.yml
- filename: boundless-bio-search-api-openapi.yml
  format: yaml
  label: Boundless Bio Search API
  slug: boundless-bio-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boundless-bio/refs/heads/main/openapi/boundless-bio-search-api-openapi.yml
- filename: boundless-bio-settings-api-openapi.yml
  format: yaml
  label: Boundless Bio Settings API
  slug: boundless-bio-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boundless-bio/refs/heads/main/openapi/boundless-bio-settings-api-openapi.yml
- filename: boundless-bio-taxonomy-api-openapi.yml
  format: yaml
  label: Boundless Bio Taxonomy API
  slug: boundless-bio-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boundless-bio/refs/heads/main/openapi/boundless-bio-taxonomy-api-openapi.yml
- filename: boundless-bio-users-api-openapi.yml
  format: yaml
  label: Boundless Bio Users API
  slug: boundless-bio-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boundless-bio/refs/heads/main/openapi/boundless-bio-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
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

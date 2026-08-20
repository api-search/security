---
api_key_in: []
api_specs:
- filename: leapcure-categories-api-openapi.yml
  format: yaml
  label: Leapcure categories API
  slug: leapcure-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapcure/refs/heads/main/openapi/leapcure-categories-api-openapi.yml
- filename: leapcure-comments-api-openapi.yml
  format: yaml
  label: Leapcure comments API
  slug: leapcure-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapcure/refs/heads/main/openapi/leapcure-comments-api-openapi.yml
- filename: leapcure-media-api-openapi.yml
  format: yaml
  label: Leapcure media API
  slug: leapcure-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapcure/refs/heads/main/openapi/leapcure-media-api-openapi.yml
- filename: leapcure-pages-api-openapi.yml
  format: yaml
  label: Leapcure pages API
  slug: leapcure-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapcure/refs/heads/main/openapi/leapcure-pages-api-openapi.yml
- filename: leapcure-posts-api-openapi.yml
  format: yaml
  label: Leapcure posts API
  slug: leapcure-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapcure/refs/heads/main/openapi/leapcure-posts-api-openapi.yml
- filename: leapcure-search-api-openapi.yml
  format: yaml
  label: Leapcure search API
  slug: leapcure-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapcure/refs/heads/main/openapi/leapcure-search-api-openapi.yml
- filename: leapcure-statuses-api-openapi.yml
  format: yaml
  label: Leapcure statuses API
  slug: leapcure-statuses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapcure/refs/heads/main/openapi/leapcure-statuses-api-openapi.yml
- filename: leapcure-tags-api-openapi.yml
  format: yaml
  label: Leapcure tags API
  slug: leapcure-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapcure/refs/heads/main/openapi/leapcure-tags-api-openapi.yml
- filename: leapcure-taxonomies-api-openapi.yml
  format: yaml
  label: Leapcure taxonomies API
  slug: leapcure-taxonomies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapcure/refs/heads/main/openapi/leapcure-taxonomies-api-openapi.yml
- filename: leapcure-types-api-openapi.yml
  format: yaml
  label: Leapcure types API
  slug: leapcure-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapcure/refs/heads/main/openapi/leapcure-types-api-openapi.yml
- filename: leapcure-users-api-openapi.yml
  format: yaml
  label: Leapcure users API
  slug: leapcure-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapcure/refs/heads/main/openapi/leapcure-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Leapcure Authentication
name_suffix: Authentication
oauth_flows: []
overview: Leapcure secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Leapcure
provider_slug: leapcure
scheme_count: 1
schemes:
- description: WordPress application passwords. Authorize at https://blog.leapcure.com/wp-admin/authorize-application.php (advertised in the /wp-json/ discovery document).
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/leapcure-blog-content-openapi.yml
  type: http
slug: leapcure-authentication
source_filename: leapcure-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/leapcure-blog-content-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: WordPress application passwords. Authorize at https://blog.leapcure.com/wp-admin/authorize-application.php\n    (advertised in the /wp-json/ discovery document).\n  sources:\n  - openapi/leapcure-blog-content-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leapcure/refs/heads/main/authentication/leapcure-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Clinical Trials
- Patient Recruitment
- Healthcare
- Blog
- content-api
- WordPress
---

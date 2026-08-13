---
api_key_in: []
api_specs:
- filename: exentis-group-posts-api-openapi.yml
  format: yaml
  label: Exentis Group Posts API
  slug: exentis-group-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exentis-group/refs/heads/main/openapi/exentis-group-posts-api-openapi.yml
- filename: exentis-group-blog-api-openapi.yml
  format: yaml
  label: Exentis Group Blog API
  slug: exentis-group-blog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exentis-group/refs/heads/main/openapi/exentis-group-blog-api-openapi.yml
- filename: exentis-group-pages-api-openapi.yml
  format: yaml
  label: Exentis Group Pages API
  slug: exentis-group-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exentis-group/refs/heads/main/openapi/exentis-group-pages-api-openapi.yml
- filename: exentis-group-media-api-openapi.yml
  format: yaml
  label: Exentis Group Media API
  slug: exentis-group-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exentis-group/refs/heads/main/openapi/exentis-group-media-api-openapi.yml
- filename: exentis-group-categories-api-openapi.yml
  format: yaml
  label: Exentis Group Categories API
  slug: exentis-group-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exentis-group/refs/heads/main/openapi/exentis-group-categories-api-openapi.yml
- filename: exentis-group-blog-categories-api-openapi.yml
  format: yaml
  label: Exentis Group Blog Categories API
  slug: exentis-group-blog-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exentis-group/refs/heads/main/openapi/exentis-group-blog-categories-api-openapi.yml
- filename: exentis-group-search-api-openapi.yml
  format: yaml
  label: Exentis Group Search API
  slug: exentis-group-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exentis-group/refs/heads/main/openapi/exentis-group-search-api-openapi.yml
- filename: exentis-group-languages-api-openapi.yml
  format: yaml
  label: Exentis Group Languages API
  slug: exentis-group-languages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exentis-group/refs/heads/main/openapi/exentis-group-languages-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Exentis Group Authentication
name_suffix: Authentication
oauth_flows: []
overview: Exentis Group secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Exentis Group
provider_slug: exentis-group
scheme_count: 1
schemes:
- description: 'WordPress application passwords (HTTP Basic: username + application password). Authorization endpoint: https://www.exentis-group.com/wp/wp-admin/authorize-application.php. Not required for the read operations documented here.'
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/exentis-group-blog-api-openapi.yml
  - openapi/exentis-group-blog-categories-api-openapi.yml
  - openapi/exentis-group-categories-api-openapi.yml
  - openapi/exentis-group-media-api-openapi.yml
  - openapi/exentis-group-pages-api-openapi.yml
  - openapi/exentis-group-posts-api-openapi.yml
  - openapi/exentis-group-search-api-openapi.yml
  type: http
slug: exentis-group-authentication
source_filename: exentis-group-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: derived\nsource: openapi/exentis-group-blog-api-openapi.yml, openapi/exentis-group-blog-categories-api-openapi.yml,\n  openapi/exentis-group-categories-api-openapi.yml, openapi/exentis-group-media-api-openapi.yml,\n  openapi/exentis-group-pages-api-openapi.yml, openapi/exentis-group-posts-api-openapi.yml,\n  openapi/exentis-group-search-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: 'WordPress application passwords (HTTP Basic: username + application password).\n    Authorization endpoint: https://www.exentis-group.com/wp/wp-admin/authorize-application.php.\n    Not required for the read operations documented here.'\n  sources:\n  - openapi/exentis-group-blog-api-openapi.yml\n  - openapi/exentis-group-blog-categories-api-openapi.yml\n  - openapi/exentis-group-categories-api-openapi.yml\n  - openapi/exentis-group-media-api-openapi.yml\n  - openapi/exentis-group-pages-api-openapi.yml\n\
  \  - openapi/exentis-group-posts-api-openapi.yml\n  - openapi/exentis-group-search-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/exentis-group/refs/heads/main/authentication/exentis-group-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Additive Manufacturing
- 3D Printing
- Industrial Manufacturing
- Advanced Materials
- Technical Ceramics
- Metals
- Pharmaceutical Manufacturing
- New Energy
- Switzerland
- Hardware
- Content
---

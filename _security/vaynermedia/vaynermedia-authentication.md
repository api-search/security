---
api_key_in: []
api_specs:
- filename: vaynermedia-blocks-api-openapi.yml
  format: yaml
  label: VaynerMedia Blocks API
  slug: vaynermedia-blocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vaynermedia/refs/heads/main/openapi/vaynermedia-blocks-api-openapi.yml
- filename: vaynermedia-casestudies-api-openapi.yml
  format: yaml
  label: VaynerMedia Case Studies API
  slug: vaynermedia-casestudies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vaynermedia/refs/heads/main/openapi/vaynermedia-casestudies-api-openapi.yml
- filename: vaynermedia-categories-api-openapi.yml
  format: yaml
  label: VaynerMedia Categories API
  slug: vaynermedia-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vaynermedia/refs/heads/main/openapi/vaynermedia-categories-api-openapi.yml
- filename: vaynermedia-comments-api-openapi.yml
  format: yaml
  label: VaynerMedia Comments API
  slug: vaynermedia-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vaynermedia/refs/heads/main/openapi/vaynermedia-comments-api-openapi.yml
- filename: vaynermedia-media-api-openapi.yml
  format: yaml
  label: VaynerMedia Media API
  slug: vaynermedia-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vaynermedia/refs/heads/main/openapi/vaynermedia-media-api-openapi.yml
- filename: vaynermedia-pages-api-openapi.yml
  format: yaml
  label: VaynerMedia Pages API
  slug: vaynermedia-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vaynermedia/refs/heads/main/openapi/vaynermedia-pages-api-openapi.yml
- filename: vaynermedia-popups-api-openapi.yml
  format: yaml
  label: VaynerMedia Popups API
  slug: vaynermedia-popups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vaynermedia/refs/heads/main/openapi/vaynermedia-popups-api-openapi.yml
- filename: vaynermedia-posts-api-openapi.yml
  format: yaml
  label: VaynerMedia Posts API
  slug: vaynermedia-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vaynermedia/refs/heads/main/openapi/vaynermedia-posts-api-openapi.yml
- filename: vaynermedia-search-api-openapi.yml
  format: yaml
  label: VaynerMedia Search API
  slug: vaynermedia-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vaynermedia/refs/heads/main/openapi/vaynermedia-search-api-openapi.yml
- filename: vaynermedia-statuses-api-openapi.yml
  format: yaml
  label: VaynerMedia Statuses API
  slug: vaynermedia-statuses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vaynermedia/refs/heads/main/openapi/vaynermedia-statuses-api-openapi.yml
- filename: vaynermedia-tags-api-openapi.yml
  format: yaml
  label: VaynerMedia Tags API
  slug: vaynermedia-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vaynermedia/refs/heads/main/openapi/vaynermedia-tags-api-openapi.yml
- filename: vaynermedia-taxonomies-api-openapi.yml
  format: yaml
  label: VaynerMedia Taxonomies API
  slug: vaynermedia-taxonomies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vaynermedia/refs/heads/main/openapi/vaynermedia-taxonomies-api-openapi.yml
- filename: vaynermedia-types-api-openapi.yml
  format: yaml
  label: VaynerMedia Types API
  slug: vaynermedia-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vaynermedia/refs/heads/main/openapi/vaynermedia-types-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Vaynermedia Authentication
name_suffix: Authentication
oauth_flows: []
overview: VaynerMedia secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: VaynerMedia
provider_slug: vaynermedia
scheme_count: 1
schemes:
- description: WordPress Application Passwords. Advertised by the site's own route index (authentication.application-passwords.endpoints.authorization = https://vaynermedia.com/wp-admin/authorize-application.php). Required only for write operations and privileged reads; every operation in this document is callable anonymously.
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/vaynermedia-wordpress-content-openapi.json
  type: http
slug: vaynermedia-authentication
source_filename: vaynermedia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: derived\nsource: openapi/vaynermedia-wordpress-content-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: WordPress Application Passwords. Advertised by the site's own route index (authentication.application-passwords.endpoints.authorization\n    = https://vaynermedia.com/wp-admin/authorize-application.php). Required only for write operations\n    and privileged reads; every operation in this document is callable anonymously.\n  sources:\n  - openapi/vaynermedia-wordpress-content-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vaynermedia/refs/heads/main/authentication/vaynermedia-authentication.yml
summary_line: http · 1 scheme
tags:
- Advertising
- Agency
- Brand Strategy
- Content Production
- Creative
- Influencer Marketing
- Marketing
- Media Buying
- Social-Media
---

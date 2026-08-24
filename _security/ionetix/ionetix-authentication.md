---
api_key_in: []
api_specs:
- filename: ionetix-posts-api-openapi.yml
  format: yaml
  label: Ionetix Posts API
  slug: ionetix-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ionetix/refs/heads/main/openapi/ionetix-posts-api-openapi.yml
- filename: ionetix-pages-api-openapi.yml
  format: yaml
  label: Ionetix Pages API
  slug: ionetix-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ionetix/refs/heads/main/openapi/ionetix-pages-api-openapi.yml
- filename: ionetix-media-api-openapi.yml
  format: yaml
  label: Ionetix Media API
  slug: ionetix-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ionetix/refs/heads/main/openapi/ionetix-media-api-openapi.yml
- filename: ionetix-taxonomy-api-openapi.yml
  format: yaml
  label: Ionetix Taxonomy API
  slug: ionetix-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ionetix/refs/heads/main/openapi/ionetix-taxonomy-api-openapi.yml
- filename: ionetix-search-api-openapi.yml
  format: yaml
  label: Ionetix Search API
  slug: ionetix-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ionetix/refs/heads/main/openapi/ionetix-search-api-openapi.yml
- filename: ionetix-users-api-openapi.yml
  format: yaml
  label: Ionetix Users API
  slug: ionetix-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ionetix/refs/heads/main/openapi/ionetix-users-api-openapi.yml
- filename: ionetix-comments-api-openapi.yml
  format: yaml
  label: Ionetix Comments API
  slug: ionetix-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ionetix/refs/heads/main/openapi/ionetix-comments-api-openapi.yml
- filename: ionetix-discovery-api-openapi.yml
  format: yaml
  label: Ionetix Discovery API
  slug: ionetix-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ionetix/refs/heads/main/openapi/ionetix-discovery-api-openapi.yml
- filename: ionetix-oembed-api-openapi.yml
  format: yaml
  label: Ionetix oEmbed API
  slug: ionetix-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ionetix/refs/heads/main/openapi/ionetix-oembed-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ionetix Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ionetix secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ionetix
provider_slug: ionetix
scheme_count: 1
schemes:
- description: WordPress Application Passwords over HTTP Basic. The route index at https://ionetix.com/wp-json/ advertises the authorization endpoint https://ionetix.com/wp-admin/authorize-application.php. Read operations on this namespace are anonymous; write operations are not.
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/ionetix-comments-api-openapi.yml
  - openapi/ionetix-discovery-api-openapi.yml
  - openapi/ionetix-media-api-openapi.yml
  - openapi/ionetix-oembed-api-openapi.yml
  - openapi/ionetix-pages-api-openapi.yml
  - openapi/ionetix-posts-api-openapi.yml
  - openapi/ionetix-search-api-openapi.yml
  - openapi/ionetix-taxonomy-api-openapi.yml
  - openapi/ionetix-users-api-openapi.yml
  type: http
slug: ionetix-authentication
source_filename: ionetix-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: derived\nsource: openapi/ionetix-comments-api-openapi.yml, openapi/ionetix-discovery-api-openapi.yml,\n  openapi/ionetix-media-api-openapi.yml, openapi/ionetix-oembed-api-openapi.yml, openapi/ionetix-pages-api-openapi.yml,\n  openapi/ionetix-posts-api-openapi.yml, openapi/ionetix-search-api-openapi.yml, openapi/ionetix-taxonomy-api-openapi.yml,\n  openapi/ionetix-users-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: WordPress Application Passwords over HTTP Basic. The route index at https://ionetix.com/wp-json/\n    advertises the authorization endpoint https://ionetix.com/wp-admin/authorize-application.php.\n    Read operations on this namespace are anonymous; write operations are not.\n  sources:\n  - openapi/ionetix-comments-api-openapi.yml\n  - openapi/ionetix-discovery-api-openapi.yml\n  - openapi/ionetix-media-api-openapi.yml\n  - openapi/ionetix-oembed-api-openapi.yml\n\
  \  - openapi/ionetix-pages-api-openapi.yml\n  - openapi/ionetix-posts-api-openapi.yml\n  - openapi/ionetix-search-api-openapi.yml\n  - openapi/ionetix-taxonomy-api-openapi.yml\n  - openapi/ionetix-users-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ionetix/refs/heads/main/authentication/ionetix-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Healthcare
- Life Sciences
- Radiopharmaceuticals
- Nuclear Medicine
- Medical Imaging
- Cardiology
- Oncology
- Isotopes
- Manufacturing
- Content
---

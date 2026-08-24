---
api_key_in: []
api_specs:
- filename: hydrostor-projects-api-openapi.yml
  format: yaml
  label: Hydrostor Projects API
  slug: hydrostor-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hydrostor/refs/heads/main/openapi/hydrostor-projects-api-openapi.yml
- filename: hydrostor-posts-api-openapi.yml
  format: yaml
  label: Hydrostor Posts API
  slug: hydrostor-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hydrostor/refs/heads/main/openapi/hydrostor-posts-api-openapi.yml
- filename: hydrostor-pages-api-openapi.yml
  format: yaml
  label: Hydrostor Pages API
  slug: hydrostor-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hydrostor/refs/heads/main/openapi/hydrostor-pages-api-openapi.yml
- filename: hydrostor-media-api-openapi.yml
  format: yaml
  label: Hydrostor Media API
  slug: hydrostor-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hydrostor/refs/heads/main/openapi/hydrostor-media-api-openapi.yml
- filename: hydrostor-taxonomy-api-openapi.yml
  format: yaml
  label: Hydrostor Taxonomy API
  slug: hydrostor-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hydrostor/refs/heads/main/openapi/hydrostor-taxonomy-api-openapi.yml
- filename: hydrostor-search-api-openapi.yml
  format: yaml
  label: Hydrostor Search API
  slug: hydrostor-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hydrostor/refs/heads/main/openapi/hydrostor-search-api-openapi.yml
- filename: hydrostor-discovery-api-openapi.yml
  format: yaml
  label: Hydrostor Discovery API
  slug: hydrostor-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hydrostor/refs/heads/main/openapi/hydrostor-discovery-api-openapi.yml
- filename: hydrostor-oembed-api-openapi.yml
  format: yaml
  label: Hydrostor oEmbed API
  slug: hydrostor-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hydrostor/refs/heads/main/openapi/hydrostor-oembed-api-openapi.yml
- filename: hydrostor-seo-api-openapi.yml
  format: yaml
  label: Hydrostor SEO Metadata API
  slug: hydrostor-seo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hydrostor/refs/heads/main/openapi/hydrostor-seo-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Hydrostor Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hydrostor secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Hydrostor
provider_slug: hydrostor
scheme_count: 1
schemes:
- description: WordPress application passwords. Issued from https://hydrostor.ca/wp-admin/authorize-application.php and advertised by the API's own root document under `authentication.application-passwords`. Required only for write and administrative routes; every read operation described in this document answers anonymously.
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/hydrostor-discovery-api-openapi.yml
  - openapi/hydrostor-media-api-openapi.yml
  - openapi/hydrostor-oembed-api-openapi.yml
  - openapi/hydrostor-pages-api-openapi.yml
  - openapi/hydrostor-posts-api-openapi.yml
  - openapi/hydrostor-projects-api-openapi.yml
  - openapi/hydrostor-search-api-openapi.yml
  - openapi/hydrostor-seo-api-openapi.yml
  - openapi/hydrostor-taxonomy-api-openapi.yml
  type: http
slug: hydrostor-authentication
source_filename: hydrostor-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: derived\nsource: openapi/hydrostor-discovery-api-openapi.yml, openapi/hydrostor-media-api-openapi.yml,\n  openapi/hydrostor-oembed-api-openapi.yml, openapi/hydrostor-pages-api-openapi.yml, openapi/hydrostor-posts-api-openapi.yml,\n  openapi/hydrostor-projects-api-openapi.yml, openapi/hydrostor-search-api-openapi.yml, openapi/hydrostor-seo-api-openapi.yml,\n  openapi/hydrostor-taxonomy-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: WordPress application passwords. Issued from https://hydrostor.ca/wp-admin/authorize-application.php\n    and advertised by the API's own root document under `authentication.application-passwords`.\n    Required only for write and administrative routes; every read operation described in this\n    document answers anonymously.\n  sources:\n  - openapi/hydrostor-discovery-api-openapi.yml\n  - openapi/hydrostor-media-api-openapi.yml\n\
  \  - openapi/hydrostor-oembed-api-openapi.yml\n  - openapi/hydrostor-pages-api-openapi.yml\n  - openapi/hydrostor-posts-api-openapi.yml\n  - openapi/hydrostor-projects-api-openapi.yml\n  - openapi/hydrostor-search-api-openapi.yml\n  - openapi/hydrostor-seo-api-openapi.yml\n  - openapi/hydrostor-taxonomy-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hydrostor/refs/heads/main/authentication/hydrostor-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Energy
- Energy Storage
- Long Duration Energy Storage
- Compressed Air Energy Storage
- Grid Infrastructure
- Renewable Energy
- Clean Energy
- Utilities
- Climate Tech
- Canada
- Content
---

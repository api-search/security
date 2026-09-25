---
anonymous_access: false
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
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
---

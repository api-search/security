---
api_key_in: []
api_specs:
- filename: housesigma-comments-api-openapi.yml
  format: yaml
  label: HouseSigma Comments API
  slug: housesigma-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/housesigma/refs/heads/main/openapi/housesigma-comments-api-openapi.yml
- filename: housesigma-media-api-openapi.yml
  format: yaml
  label: HouseSigma Media API
  slug: housesigma-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/housesigma/refs/heads/main/openapi/housesigma-media-api-openapi.yml
- filename: housesigma-oembed-api-openapi.yml
  format: yaml
  label: HouseSigma O Embed API
  slug: housesigma-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/housesigma/refs/heads/main/openapi/housesigma-oembed-api-openapi.yml
- filename: housesigma-pages-api-openapi.yml
  format: yaml
  label: HouseSigma Pages API
  slug: housesigma-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/housesigma/refs/heads/main/openapi/housesigma-pages-api-openapi.yml
- filename: housesigma-posts-api-openapi.yml
  format: yaml
  label: HouseSigma Posts API
  slug: housesigma-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/housesigma/refs/heads/main/openapi/housesigma-posts-api-openapi.yml
- filename: housesigma-search-api-openapi.yml
  format: yaml
  label: HouseSigma Search API
  slug: housesigma-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/housesigma/refs/heads/main/openapi/housesigma-search-api-openapi.yml
- filename: housesigma-taxonomies-api-openapi.yml
  format: yaml
  label: HouseSigma Taxonomies API
  slug: housesigma-taxonomies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/housesigma/refs/heads/main/openapi/housesigma-taxonomies-api-openapi.yml
- filename: housesigma-types-api-openapi.yml
  format: yaml
  label: HouseSigma Types API
  slug: housesigma-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/housesigma/refs/heads/main/openapi/housesigma-types-api-openapi.yml
- filename: housesigma-users-api-openapi.yml
  format: yaml
  label: HouseSigma Users API
  slug: housesigma-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/housesigma/refs/heads/main/openapi/housesigma-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Housesigma Authentication
name_suffix: Authentication
oauth_flows: []
overview: HouseSigma secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: HouseSigma
provider_slug: housesigma
scheme_count: 1
schemes:
- description: WordPress application passwords, advertised by the live discovery document at https://housesigma.com/blog-en/wp-admin/authorize-application.php. Required only for write methods and for routes excluded from this document; every operation modelled here is anonymous.
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/housesigma-blog-content-openapi.yml
  type: http
slug: housesigma-authentication
source_filename: housesigma-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: derived\nsource: openapi/housesigma-blog-content-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: WordPress application passwords, advertised by the live discovery document at\n    https://housesigma.com/blog-en/wp-admin/authorize-application.php. Required only for write\n    methods and for routes excluded from this document; every operation modelled here is anonymous.\n  sources:\n  - openapi/housesigma-blog-content-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/housesigma/refs/heads/main/authentication/housesigma-authentication.yml
summary_line: http · 1 scheme
tags:
- Real-Estate
- Canada
- Property Listings
- MLS
- Valuation
- AVM
- PropTech
- Rentals
- Blog
- Content
- WordPress
- oEmbed
- Ontario
- British Columbia
- Toronto
---

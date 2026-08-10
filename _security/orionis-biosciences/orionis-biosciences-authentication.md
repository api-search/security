---
api_key_in:
- header
api_specs:
- filename: orionis-biosciences-abilities-api-openapi.yml
  format: yaml
  label: Orionis Biosciences Abilities API
  slug: orionis-biosciences-abilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orionis-biosciences/refs/heads/main/openapi/orionis-biosciences-abilities-api-openapi.yml
- filename: orionis-biosciences-comments-api-openapi.yml
  format: yaml
  label: Orionis Biosciences Comments API
  slug: orionis-biosciences-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orionis-biosciences/refs/heads/main/openapi/orionis-biosciences-comments-api-openapi.yml
- filename: orionis-biosciences-discovery-api-openapi.yml
  format: yaml
  label: Orionis Biosciences Discovery API
  slug: orionis-biosciences-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orionis-biosciences/refs/heads/main/openapi/orionis-biosciences-discovery-api-openapi.yml
- filename: orionis-biosciences-media-api-openapi.yml
  format: yaml
  label: Orionis Biosciences Media API
  slug: orionis-biosciences-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orionis-biosciences/refs/heads/main/openapi/orionis-biosciences-media-api-openapi.yml
- filename: orionis-biosciences-news-api-openapi.yml
  format: yaml
  label: Orionis Biosciences News API
  slug: orionis-biosciences-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orionis-biosciences/refs/heads/main/openapi/orionis-biosciences-news-api-openapi.yml
- filename: orionis-biosciences-oembed-api-openapi.yml
  format: yaml
  label: Orionis Biosciences O Embed API
  slug: orionis-biosciences-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orionis-biosciences/refs/heads/main/openapi/orionis-biosciences-oembed-api-openapi.yml
- filename: orionis-biosciences-pages-api-openapi.yml
  format: yaml
  label: Orionis Biosciences Pages API
  slug: orionis-biosciences-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orionis-biosciences/refs/heads/main/openapi/orionis-biosciences-pages-api-openapi.yml
- filename: orionis-biosciences-search-api-openapi.yml
  format: yaml
  label: Orionis Biosciences Search API
  slug: orionis-biosciences-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orionis-biosciences/refs/heads/main/openapi/orionis-biosciences-search-api-openapi.yml
- filename: orionis-biosciences-taxonomy-api-openapi.yml
  format: yaml
  label: Orionis Biosciences Taxonomy API
  slug: orionis-biosciences-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orionis-biosciences/refs/heads/main/openapi/orionis-biosciences-taxonomy-api-openapi.yml
- filename: orionis-biosciences-team-api-openapi.yml
  format: yaml
  label: Orionis Biosciences Team API
  slug: orionis-biosciences-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orionis-biosciences/refs/heads/main/openapi/orionis-biosciences-team-api-openapi.yml
- filename: orionis-biosciences-users-api-openapi.yml
  format: yaml
  label: Orionis Biosciences Users API
  slug: orionis-biosciences-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orionis-biosciences/refs/heads/main/openapi/orionis-biosciences-users-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Orionis Biosciences Authentication
name_suffix: Authentication
oauth_flows: []
overview: Orionis Biosciences secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Orionis Biosciences
provider_slug: orionis-biosciences
scheme_count: 2
schemes:
- description: WordPress Application Passwords (RFC 7617 Basic). The site advertises the authorization endpoint https://orionisbio.com/wp-admin/authorize-application.php in its /wp-json/ root document. Write access only; not issued to the public.
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/orionis-biosciences-content-openapi.yml
  type: http
- description: WordPress cookie authentication with an X-WP-Nonce header (first-party browser context only).
  in: header
  name: cookieNonce
  parameter: X-WP-Nonce
  sources:
  - openapi/orionis-biosciences-content-openapi.yml
  type: apiKey
slug: orionis-biosciences-authentication
source_filename: orionis-biosciences-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: derived\nsource: openapi/orionis-biosciences-content-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: WordPress Application Passwords (RFC 7617 Basic). The site advertises the authorization\n    endpoint https://orionisbio.com/wp-admin/authorize-application.php in its /wp-json/ root\n    document. Write access only; not issued to the public.\n  sources:\n  - openapi/orionis-biosciences-content-openapi.yml\n- name: cookieNonce\n  type: apiKey\n  in: header\n  parameter: X-WP-Nonce\n  description: WordPress cookie authentication with an X-WP-Nonce header (first-party browser\n    context only).\n  sources:\n  - openapi/orionis-biosciences-content-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orionis-biosciences/refs/heads/main/authentication/orionis-biosciences-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Biotechnology
- Life Sciences
- Drug Discovery
- Pharmaceuticals
- Oncology
- Immunotherapy
- Protein Engineering
- Molecular Glues
- Computational Biology
- Machine Learning
- Clinical Trials
- Content
---

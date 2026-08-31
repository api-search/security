---
api_key_in:
- header
api_specs:
- filename: habiteo-posts-api-openapi.yml
  format: yaml
  label: Habiteo Site Content API — Posts API
  slug: posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/habiteo/refs/heads/main/openapi/habiteo-posts-api-openapi.yml
- filename: habiteo-pages-api-openapi.yml
  format: yaml
  label: Habiteo Site Content API — Pages API
  slug: pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/habiteo/refs/heads/main/openapi/habiteo-pages-api-openapi.yml
- filename: habiteo-media-api-openapi.yml
  format: yaml
  label: Habiteo Site Content API — Media API
  slug: media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/habiteo/refs/heads/main/openapi/habiteo-media-api-openapi.yml
- filename: habiteo-portfolio-api-openapi.yml
  format: yaml
  label: Habiteo Site Content API — Portfolio API
  slug: portfolio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/habiteo/refs/heads/main/openapi/habiteo-portfolio-api-openapi.yml
- filename: habiteo-blocks-api-openapi.yml
  format: yaml
  label: Habiteo Site Content API — Blocks API
  slug: blocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/habiteo/refs/heads/main/openapi/habiteo-blocks-api-openapi.yml
- filename: habiteo-taxonomy-api-openapi.yml
  format: yaml
  label: Habiteo Site Content API — Taxonomy API
  slug: taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/habiteo/refs/heads/main/openapi/habiteo-taxonomy-api-openapi.yml
- filename: habiteo-discovery-api-openapi.yml
  format: yaml
  label: Habiteo Site Content API — Discovery API
  slug: discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/habiteo/refs/heads/main/openapi/habiteo-discovery-api-openapi.yml
- filename: habiteo-users-api-openapi.yml
  format: yaml
  label: Habiteo Site Content API — Users API
  slug: users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/habiteo/refs/heads/main/openapi/habiteo-users-api-openapi.yml
- filename: habiteo-comments-api-openapi.yml
  format: yaml
  label: Habiteo Site Content API — Comments API
  slug: comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/habiteo/refs/heads/main/openapi/habiteo-comments-api-openapi.yml
- filename: habiteo-settings-api-openapi.yml
  format: yaml
  label: Habiteo Site Content API — Settings API
  slug: settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/habiteo/refs/heads/main/openapi/habiteo-settings-api-openapi.yml
- filename: habiteo-oembed-api-openapi.yml
  format: yaml
  label: Habiteo Site Content API — oEmbed API
  slug: oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/habiteo/refs/heads/main/openapi/habiteo-oembed-api-openapi.yml
- filename: habiteo-contactforms-api-openapi.yml
  format: yaml
  label: Habiteo Contact Forms API
  slug: habiteo-contactforms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/habiteo/refs/heads/main/openapi/habiteo-contactforms-api-openapi.yml
- filename: habiteo-sitetools-api-openapi.yml
  format: yaml
  label: Habiteo Site Tools API
  slug: habiteo-sitetools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/habiteo/refs/heads/main/openapi/habiteo-sitetools-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Habiteo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Habiteo secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Habiteo
provider_slug: habiteo
scheme_count: 2
schemes:
- description: WordPress Application Passwords over HTTP Basic. Required for every write operation.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/habiteo-blocks-api-openapi.yml
  - openapi/habiteo-comments-api-openapi.yml
  - openapi/habiteo-contact-forms-api-openapi.yml
  - openapi/habiteo-discovery-api-openapi.yml
  - openapi/habiteo-media-api-openapi.yml
  - openapi/habiteo-oembed-api-openapi.yml
  - openapi/habiteo-pages-api-openapi.yml
  - openapi/habiteo-portfolio-api-openapi.yml
  - openapi/habiteo-posts-api-openapi.yml
  - openapi/habiteo-settings-api-openapi.yml
  - openapi/habiteo-site-tools-api-openapi.yml
  - openapi/habiteo-taxonomy-api-openapi.yml
  - openapi/habiteo-users-api-openapi.yml
  type: http
- description: WordPress logged-in cookie plus an X-WP-Nonce header, used by first-party admin clients.
  in: header
  name: cookieNonce
  parameter: X-WP-Nonce
  sources:
  - openapi/habiteo-blocks-api-openapi.yml
  - openapi/habiteo-comments-api-openapi.yml
  - openapi/habiteo-contact-forms-api-openapi.yml
  - openapi/habiteo-discovery-api-openapi.yml
  - openapi/habiteo-media-api-openapi.yml
  - openapi/habiteo-oembed-api-openapi.yml
  - openapi/habiteo-pages-api-openapi.yml
  - openapi/habiteo-portfolio-api-openapi.yml
  - openapi/habiteo-posts-api-openapi.yml
  - openapi/habiteo-settings-api-openapi.yml
  - openapi/habiteo-site-tools-api-openapi.yml
  - openapi/habiteo-taxonomy-api-openapi.yml
  - openapi/habiteo-users-api-openapi.yml
  type: apiKey
slug: habiteo-authentication
source_filename: habiteo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: derived\nsource: openapi/habiteo-blocks-api-openapi.yml, openapi/habiteo-comments-api-openapi.yml, openapi/habiteo-contact-forms-api-openapi.yml,\n  openapi/habiteo-discovery-api-openapi.yml, openapi/habiteo-media-api-openapi.yml, openapi/habiteo-oembed-api-openapi.yml,\n  openapi/habiteo-pages-api-openapi.yml, openapi/habiteo-portfolio-api-openapi.yml, openapi/habiteo-posts-api-openapi.yml,\n  openapi/habiteo-settings-api-openapi.yml, openapi/habiteo-site-tools-api-openapi.yml, openapi/habiteo-taxonomy-api-openapi.yml\n  ...\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: WordPress Application Passwords over HTTP Basic. Required for every write operation.\n  sources:\n  - openapi/habiteo-blocks-api-openapi.yml\n  - openapi/habiteo-comments-api-openapi.yml\n  - openapi/habiteo-contact-forms-api-openapi.yml\n  - openapi/habiteo-discovery-api-openapi.yml\n\
  \  - openapi/habiteo-media-api-openapi.yml\n  - openapi/habiteo-oembed-api-openapi.yml\n  - openapi/habiteo-pages-api-openapi.yml\n  - openapi/habiteo-portfolio-api-openapi.yml\n  - openapi/habiteo-posts-api-openapi.yml\n  - openapi/habiteo-settings-api-openapi.yml\n  - openapi/habiteo-site-tools-api-openapi.yml\n  - openapi/habiteo-taxonomy-api-openapi.yml\n  - openapi/habiteo-users-api-openapi.yml\n- name: cookieNonce\n  type: apiKey\n  in: header\n  parameter: X-WP-Nonce\n  description: WordPress logged-in cookie plus an X-WP-Nonce header, used by first-party admin\n    clients.\n  sources:\n  - openapi/habiteo-blocks-api-openapi.yml\n  - openapi/habiteo-comments-api-openapi.yml\n  - openapi/habiteo-contact-forms-api-openapi.yml\n  - openapi/habiteo-discovery-api-openapi.yml\n  - openapi/habiteo-media-api-openapi.yml\n  - openapi/habiteo-oembed-api-openapi.yml\n  - openapi/habiteo-pages-api-openapi.yml\n  - openapi/habiteo-portfolio-api-openapi.yml\n  - openapi/habiteo-posts-api-openapi.yml\n\
  \  - openapi/habiteo-settings-api-openapi.yml\n  - openapi/habiteo-site-tools-api-openapi.yml\n  - openapi/habiteo-taxonomy-api-openapi.yml\n  - openapi/habiteo-users-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/habiteo/refs/heads/main/authentication/habiteo-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Real-Estate
- PropTech
- 3D Visualization
- Property Marketing
- Configurator
- CRM
- France
- Content
- WordPress
---

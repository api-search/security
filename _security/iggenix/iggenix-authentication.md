---
api_key_in: []
api_specs:
- filename: iggenix-press-releases-api-openapi.yml
  format: yaml
  label: IgGenix Press Releases API
  slug: iggenix-press-releases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iggenix/refs/heads/main/openapi/iggenix-press-releases-api-openapi.yml
- filename: iggenix-publications-api-openapi.yml
  format: yaml
  label: IgGenix Publications API
  slug: iggenix-publications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iggenix/refs/heads/main/openapi/iggenix-publications-api-openapi.yml
- filename: iggenix-abstracts-api-openapi.yml
  format: yaml
  label: IgGenix Abstracts API
  slug: iggenix-abstracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iggenix/refs/heads/main/openapi/iggenix-abstracts-api-openapi.yml
- filename: iggenix-careers-api-openapi.yml
  format: yaml
  label: IgGenix Careers API
  slug: iggenix-careers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iggenix/refs/heads/main/openapi/iggenix-careers-api-openapi.yml
- filename: iggenix-posts-api-openapi.yml
  format: yaml
  label: IgGenix Posts API
  slug: iggenix-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iggenix/refs/heads/main/openapi/iggenix-posts-api-openapi.yml
- filename: iggenix-pages-api-openapi.yml
  format: yaml
  label: IgGenix Pages API
  slug: iggenix-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iggenix/refs/heads/main/openapi/iggenix-pages-api-openapi.yml
- filename: iggenix-media-api-openapi.yml
  format: yaml
  label: IgGenix Media API
  slug: iggenix-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iggenix/refs/heads/main/openapi/iggenix-media-api-openapi.yml
- filename: iggenix-comments-api-openapi.yml
  format: yaml
  label: IgGenix Comments API
  slug: iggenix-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iggenix/refs/heads/main/openapi/iggenix-comments-api-openapi.yml
- filename: iggenix-taxonomy-api-openapi.yml
  format: yaml
  label: IgGenix Taxonomy API
  slug: iggenix-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iggenix/refs/heads/main/openapi/iggenix-taxonomy-api-openapi.yml
- filename: iggenix-search-api-openapi.yml
  format: yaml
  label: IgGenix Search API
  slug: iggenix-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iggenix/refs/heads/main/openapi/iggenix-search-api-openapi.yml
- filename: iggenix-users-api-openapi.yml
  format: yaml
  label: IgGenix Users API
  slug: iggenix-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iggenix/refs/heads/main/openapi/iggenix-users-api-openapi.yml
- filename: iggenix-settings-api-openapi.yml
  format: yaml
  label: IgGenix Settings API
  slug: iggenix-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iggenix/refs/heads/main/openapi/iggenix-settings-api-openapi.yml
- filename: iggenix-discovery-api-openapi.yml
  format: yaml
  label: IgGenix Discovery API
  slug: iggenix-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iggenix/refs/heads/main/openapi/iggenix-discovery-api-openapi.yml
- filename: iggenix-oembed-api-openapi.yml
  format: yaml
  label: IgGenix oEmbed API
  slug: iggenix-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iggenix/refs/heads/main/openapi/iggenix-oembed-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Iggenix Authentication
name_suffix: Authentication
oauth_flows: []
overview: IgGenix secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: IgGenix
provider_slug: iggenix
scheme_count: 1
schemes:
- description: WordPress Application Passwords over HTTP Basic. Advertised by the site's own route index at https://iggenix.com/wp-json/ under authentication.application-passwords, with the authorization endpoint at https://iggenix.com/wp-admin/authorize-application.php. Required only for write operations and for the authenticated-read routes (/wp/v2/settings, /wp-abilities/v1/*); the content read surface is ano
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/iggenix-abstracts-api-openapi.yml
  - openapi/iggenix-careers-api-openapi.yml
  - openapi/iggenix-comments-api-openapi.yml
  - openapi/iggenix-discovery-api-openapi.yml
  - openapi/iggenix-media-api-openapi.yml
  - openapi/iggenix-oembed-api-openapi.yml
  - openapi/iggenix-pages-api-openapi.yml
  - openapi/iggenix-posts-api-openapi.yml
  - openapi/iggenix-press-releases-api-openapi.yml
  - openapi/iggenix-publications-api-openapi.yml
  - openapi/iggenix-search-api-openapi.yml
  - openapi/iggenix-settings-api-openapi.yml
  - openapi/iggenix-taxonomy-api-openapi.yml
  - openapi/iggenix-users-api-openapi.yml
  type: http
slug: iggenix-authentication
source_filename: iggenix-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: derived\nsource: openapi/iggenix-abstracts-api-openapi.yml, openapi/iggenix-careers-api-openapi.yml,\n  openapi/iggenix-comments-api-openapi.yml, openapi/iggenix-discovery-api-openapi.yml, openapi/iggenix-media-api-openapi.yml,\n  openapi/iggenix-oembed-api-openapi.yml, openapi/iggenix-pages-api-openapi.yml, openapi/iggenix-posts-api-openapi.yml,\n  openapi/iggenix-press-releases-api-openapi.yml, openapi/iggenix-publications-api-openapi.yml,\n  openapi/iggenix-search-api-openapi.yml, openapi/iggenix-settings-api-openapi.yml ...\nsummary:\n  types:\n  - http\nschemes:\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: WordPress Application Passwords over HTTP Basic. Advertised by the site's own\n    route index at https://iggenix.com/wp-json/ under authentication.application-passwords,\n    with the authorization endpoint at https://iggenix.com/wp-admin/authorize-application.php.\n    Required only for write operations\
  \ and for the authenticated-read routes (/wp/v2/settings,\n    /wp-abilities/v1/*); the content read surface is ano\n  sources:\n  - openapi/iggenix-abstracts-api-openapi.yml\n  - openapi/iggenix-careers-api-openapi.yml\n  - openapi/iggenix-comments-api-openapi.yml\n  - openapi/iggenix-discovery-api-openapi.yml\n  - openapi/iggenix-media-api-openapi.yml\n  - openapi/iggenix-oembed-api-openapi.yml\n  - openapi/iggenix-pages-api-openapi.yml\n  - openapi/iggenix-posts-api-openapi.yml\n  - openapi/iggenix-press-releases-api-openapi.yml\n  - openapi/iggenix-publications-api-openapi.yml\n  - openapi/iggenix-search-api-openapi.yml\n  - openapi/iggenix-settings-api-openapi.yml\n  - openapi/iggenix-taxonomy-api-openapi.yml\n  - openapi/iggenix-users-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iggenix/refs/heads/main/authentication/iggenix-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Biotechnology
- Life Sciences
- Immunology
- Allergy
- Antibodies
- Drug Discovery
- Therapeutics
- Clinical Trials
- Pharmaceuticals
- Research
- Content
---

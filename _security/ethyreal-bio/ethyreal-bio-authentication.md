---
api_key_in: []
api_specs:
- filename: ethyreal-bio-comments-api-openapi.yml
  format: yaml
  label: Ethyreal Bio Comments API
  slug: ethyreal-bio-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ethyreal-bio/refs/heads/main/openapi/ethyreal-bio-comments-api-openapi.yml
- filename: ethyreal-bio-discovery-api-openapi.yml
  format: yaml
  label: Ethyreal Bio Discovery API
  slug: ethyreal-bio-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ethyreal-bio/refs/heads/main/openapi/ethyreal-bio-discovery-api-openapi.yml
- filename: ethyreal-bio-faq-api-openapi.yml
  format: yaml
  label: Ethyreal Bio FAQ API
  slug: ethyreal-bio-faq-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ethyreal-bio/refs/heads/main/openapi/ethyreal-bio-faq-api-openapi.yml
- filename: ethyreal-bio-media-api-openapi.yml
  format: yaml
  label: Ethyreal Bio Media API
  slug: ethyreal-bio-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ethyreal-bio/refs/heads/main/openapi/ethyreal-bio-media-api-openapi.yml
- filename: ethyreal-bio-news-api-openapi.yml
  format: yaml
  label: Ethyreal Bio News API
  slug: ethyreal-bio-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ethyreal-bio/refs/heads/main/openapi/ethyreal-bio-news-api-openapi.yml
- filename: ethyreal-bio-pages-api-openapi.yml
  format: yaml
  label: Ethyreal Bio Pages API
  slug: ethyreal-bio-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ethyreal-bio/refs/heads/main/openapi/ethyreal-bio-pages-api-openapi.yml
- filename: ethyreal-bio-people-api-openapi.yml
  format: yaml
  label: Ethyreal Bio People API
  slug: ethyreal-bio-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ethyreal-bio/refs/heads/main/openapi/ethyreal-bio-people-api-openapi.yml
- filename: ethyreal-bio-portfolio-api-openapi.yml
  format: yaml
  label: Ethyreal Bio Portfolio API
  slug: ethyreal-bio-portfolio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ethyreal-bio/refs/heads/main/openapi/ethyreal-bio-portfolio-api-openapi.yml
- filename: ethyreal-bio-search-api-openapi.yml
  format: yaml
  label: Ethyreal Bio Search API
  slug: ethyreal-bio-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ethyreal-bio/refs/heads/main/openapi/ethyreal-bio-search-api-openapi.yml
- filename: ethyreal-bio-settings-api-openapi.yml
  format: yaml
  label: Ethyreal Bio Settings API
  slug: ethyreal-bio-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ethyreal-bio/refs/heads/main/openapi/ethyreal-bio-settings-api-openapi.yml
- filename: ethyreal-bio-taxonomy-api-openapi.yml
  format: yaml
  label: Ethyreal Bio Taxonomy API
  slug: ethyreal-bio-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ethyreal-bio/refs/heads/main/openapi/ethyreal-bio-taxonomy-api-openapi.yml
- filename: ethyreal-bio-users-api-openapi.yml
  format: yaml
  label: Ethyreal Bio Users API
  slug: ethyreal-bio-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ethyreal-bio/refs/heads/main/openapi/ethyreal-bio-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ethyreal Bio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ethyreal Bio secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ethyreal Bio
provider_slug: ethyreal-bio
scheme_count: 1
schemes:
- description: WordPress Application Passwords, advertised by the site at https://www.ethyrealbio.com/wp-json/ under authentication.application-passwords; authorization endpoint https://www.ethyrealbio.com/wp-admin/authorize-application.php. Read operations on wp/v2 content routes are anonymous.
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/ethyreal-bio-comments-api-openapi.yml
  - openapi/ethyreal-bio-discovery-api-openapi.yml
  - openapi/ethyreal-bio-faq-api-openapi.yml
  - openapi/ethyreal-bio-media-api-openapi.yml
  - openapi/ethyreal-bio-news-api-openapi.yml
  - openapi/ethyreal-bio-pages-api-openapi.yml
  - openapi/ethyreal-bio-people-api-openapi.yml
  - openapi/ethyreal-bio-portfolio-api-openapi.yml
  - openapi/ethyreal-bio-search-api-openapi.yml
  - openapi/ethyreal-bio-settings-api-openapi.yml
  - openapi/ethyreal-bio-taxonomy-api-openapi.yml
  - openapi/ethyreal-bio-users-api-openapi.yml
  type: http
slug: ethyreal-bio-authentication
source_filename: ethyreal-bio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: derived\nsource: openapi/ethyreal-bio-comments-api-openapi.yml, openapi/ethyreal-bio-discovery-api-openapi.yml,\n  openapi/ethyreal-bio-faq-api-openapi.yml, openapi/ethyreal-bio-media-api-openapi.yml, openapi/ethyreal-bio-news-api-openapi.yml,\n  openapi/ethyreal-bio-pages-api-openapi.yml, openapi/ethyreal-bio-people-api-openapi.yml, openapi/ethyreal-bio-portfolio-api-openapi.yml,\n  openapi/ethyreal-bio-search-api-openapi.yml, openapi/ethyreal-bio-settings-api-openapi.yml,\n  openapi/ethyreal-bio-taxonomy-api-openapi.yml, openapi/ethyreal-bio-users-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: WordPress Application Passwords, advertised by the site at https://www.ethyrealbio.com/wp-json/\n    under authentication.application-passwords; authorization endpoint https://www.ethyrealbio.com/wp-admin/authorize-application.php.\n    Read operations on wp/v2 content\
  \ routes are anonymous.\n  sources:\n  - openapi/ethyreal-bio-comments-api-openapi.yml\n  - openapi/ethyreal-bio-discovery-api-openapi.yml\n  - openapi/ethyreal-bio-faq-api-openapi.yml\n  - openapi/ethyreal-bio-media-api-openapi.yml\n  - openapi/ethyreal-bio-news-api-openapi.yml\n  - openapi/ethyreal-bio-pages-api-openapi.yml\n  - openapi/ethyreal-bio-people-api-openapi.yml\n  - openapi/ethyreal-bio-portfolio-api-openapi.yml\n  - openapi/ethyreal-bio-search-api-openapi.yml\n  - openapi/ethyreal-bio-settings-api-openapi.yml\n  - openapi/ethyreal-bio-taxonomy-api-openapi.yml\n  - openapi/ethyreal-bio-users-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ethyreal-bio/refs/heads/main/authentication/ethyreal-bio-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Life Sciences
- Drug Discovery
- Clinical Trials
- Immunology
- Endocrinology
- Antibodies
- Rare Disease
- Health
- Content
---

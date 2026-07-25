---
api_key_in:
- cookie
api_specs:
- filename: wikivoyage-authentication-api-openapi.yml
  format: yaml
  label: Wikivoyage Authentication API
  slug: wikivoyage-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikivoyage/refs/heads/main/openapi/wikivoyage-authentication-api-openapi.yml
- filename: wikivoyage-edit-api-openapi.yml
  format: yaml
  label: Wikivoyage Edit API
  slug: wikivoyage-edit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikivoyage/refs/heads/main/openapi/wikivoyage-edit-api-openapi.yml
- filename: wikivoyage-files-api-openapi.yml
  format: yaml
  label: Wikivoyage Files API
  slug: wikivoyage-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikivoyage/refs/heads/main/openapi/wikivoyage-files-api-openapi.yml
- filename: wikivoyage-history-api-openapi.yml
  format: yaml
  label: Wikivoyage History API
  slug: wikivoyage-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikivoyage/refs/heads/main/openapi/wikivoyage-history-api-openapi.yml
- filename: wikivoyage-links-api-openapi.yml
  format: yaml
  label: Wikivoyage Links API
  slug: wikivoyage-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikivoyage/refs/heads/main/openapi/wikivoyage-links-api-openapi.yml
- filename: wikivoyage-meta-api-openapi.yml
  format: yaml
  label: Wikivoyage Meta API
  slug: wikivoyage-meta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikivoyage/refs/heads/main/openapi/wikivoyage-meta-api-openapi.yml
- filename: wikivoyage-pages-api-openapi.yml
  format: yaml
  label: Wikivoyage Pages API
  slug: wikivoyage-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikivoyage/refs/heads/main/openapi/wikivoyage-pages-api-openapi.yml
- filename: wikivoyage-parse-api-openapi.yml
  format: yaml
  label: Wikivoyage Parse API
  slug: wikivoyage-parse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikivoyage/refs/heads/main/openapi/wikivoyage-parse-api-openapi.yml
- filename: wikivoyage-patrol-api-openapi.yml
  format: yaml
  label: Wikivoyage Patrol API
  slug: wikivoyage-patrol-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikivoyage/refs/heads/main/openapi/wikivoyage-patrol-api-openapi.yml
- filename: wikivoyage-query-api-openapi.yml
  format: yaml
  label: Wikivoyage Query API
  slug: wikivoyage-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikivoyage/refs/heads/main/openapi/wikivoyage-query-api-openapi.yml
- filename: wikivoyage-revisions-api-openapi.yml
  format: yaml
  label: Wikivoyage Revisions API
  slug: wikivoyage-revisions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikivoyage/refs/heads/main/openapi/wikivoyage-revisions-api-openapi.yml
- filename: wikivoyage-search-api-openapi.yml
  format: yaml
  label: Wikivoyage Search API
  slug: wikivoyage-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikivoyage/refs/heads/main/openapi/wikivoyage-search-api-openapi.yml
- filename: wikivoyage-transforms-api-openapi.yml
  format: yaml
  label: Wikivoyage Transforms API
  slug: wikivoyage-transforms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikivoyage/refs/heads/main/openapi/wikivoyage-transforms-api-openapi.yml
- filename: wikivoyage-upload-api-openapi.yml
  format: yaml
  label: Wikivoyage Upload API
  slug: wikivoyage-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikivoyage/refs/heads/main/openapi/wikivoyage-upload-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Wikivoyage Authentication
name_suffix: Authentication
oauth_flows: []
overview: Wikivoyage secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Wikivoyage
provider_slug: wikivoyage
scheme_count: 2
schemes:
- description: OAuth 2.0 bearer token from meta.wikimedia.org
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/wikivoyage-mediawiki-action-api-openapi.yaml
  - openapi/wikivoyage-mediawiki-core-rest-openapi.yaml
  type: http
- description: Session cookie obtained via action=login or action=clientlogin
  in: cookie
  name: CookieAuth
  parameter: wikivoyagewikiUserID
  sources:
  - openapi/wikivoyage-mediawiki-action-api-openapi.yaml
  type: apiKey
slug: wikivoyage-authentication
source_filename: wikivoyage-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/wikivoyage-mediawiki-action-api-openapi.yaml, openapi/wikivoyage-mediawiki-core-rest-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 bearer token from meta.wikimedia.org\n  sources:\n  - openapi/wikivoyage-mediawiki-action-api-openapi.yaml\n  - openapi/wikivoyage-mediawiki-core-rest-openapi.yaml\n- name: CookieAuth\n  type: apiKey\n  in: cookie\n  parameter: wikivoyagewikiUserID\n  description: Session cookie obtained via action=login or action=clientlogin\n  sources:\n  - openapi/wikivoyage-mediawiki-action-api-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wikivoyage/refs/heads/main/authentication/wikivoyage-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Travel
- Open Data
- Public APIs
- Open Knowledge
- Travel Guide
- Tourism
- MediaWiki
- Non-Profit
---

---
api_key_in:
- cookie
api_specs:
- filename: wikivoyage-mediawiki-action-api-openapi.yaml
  format: yaml
  label: Wikivoyage MediaWiki Action API
  slug: wikivoyage-mediawiki-action-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikivoyage/refs/heads/main/openapi/wikivoyage-mediawiki-action-api-openapi.yaml
- filename: wikivoyage-mediawiki-core-rest-openapi.yaml
  format: yaml
  label: Wikivoyage MediaWiki Core REST API
  slug: wikivoyage-mediawiki-core-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikivoyage/refs/heads/main/openapi/wikivoyage-mediawiki-core-rest-openapi.yaml
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

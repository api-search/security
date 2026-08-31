---
api_key_in:
- cookie
api_specs:
- filename: wikipedia-articles-api-openapi.yml
  format: yaml
  label: Wikipedia / MediaWiki articles API
  slug: wikipedia-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikipedia/refs/heads/main/openapi/wikipedia-articles-api-openapi.yml
- filename: wikipedia-batches-api-openapi.yml
  format: yaml
  label: Wikipedia / MediaWiki batches API
  slug: wikipedia-batches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikipedia/refs/heads/main/openapi/wikipedia-batches-api-openapi.yml
- filename: wikipedia-citation-api-openapi.yml
  format: yaml
  label: Wikipedia / MediaWiki Citation API
  slug: wikipedia-citation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikipedia/refs/heads/main/openapi/wikipedia-citation-api-openapi.yml
- filename: wikipedia-codes-api-openapi.yml
  format: yaml
  label: Wikipedia / MediaWiki codes API
  slug: wikipedia-codes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikipedia/refs/heads/main/openapi/wikipedia-codes-api-openapi.yml
- filename: wikipedia-languages-api-openapi.yml
  format: yaml
  label: Wikipedia / MediaWiki languages API
  slug: wikipedia-languages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikipedia/refs/heads/main/openapi/wikipedia-languages-api-openapi.yml
- filename: wikipedia-math-api-openapi.yml
  format: yaml
  label: Wikipedia / MediaWiki Math API
  slug: wikipedia-math-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikipedia/refs/heads/main/openapi/wikipedia-math-api-openapi.yml
- filename: wikipedia-mobile-api-openapi.yml
  format: yaml
  label: Wikipedia / MediaWiki Mobile API
  slug: wikipedia-mobile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikipedia/refs/heads/main/openapi/wikipedia-mobile-api-openapi.yml
- filename: wikipedia-namespaces-api-openapi.yml
  format: yaml
  label: Wikipedia / MediaWiki namespaces API
  slug: wikipedia-namespaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikipedia/refs/heads/main/openapi/wikipedia-namespaces-api-openapi.yml
- filename: wikipedia-offline-api-openapi.yml
  format: yaml
  label: Wikipedia / MediaWiki offline API
  slug: wikipedia-offline-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikipedia/refs/heads/main/openapi/wikipedia-offline-api-openapi.yml
- filename: wikipedia-page-content-api-openapi.yml
  format: yaml
  label: Wikipedia / MediaWiki Page content API
  slug: wikipedia-page-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikipedia/refs/heads/main/openapi/wikipedia-page-content-api-openapi.yml
- filename: wikipedia-projects-api-openapi.yml
  format: yaml
  label: Wikipedia / MediaWiki projects API
  slug: wikipedia-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikipedia/refs/heads/main/openapi/wikipedia-projects-api-openapi.yml
- filename: wikipedia-reading-lists-api-openapi.yml
  format: yaml
  label: Wikipedia / MediaWiki Reading lists API
  slug: wikipedia-reading-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikipedia/refs/heads/main/openapi/wikipedia-reading-lists-api-openapi.yml
- filename: wikipedia-recommendation-api-openapi.yml
  format: yaml
  label: Wikipedia / MediaWiki Recommendation API
  slug: wikipedia-recommendation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikipedia/refs/heads/main/openapi/wikipedia-recommendation-api-openapi.yml
- filename: wikipedia-snapshots-api-openapi.yml
  format: yaml
  label: Wikipedia / MediaWiki snapshots API
  slug: wikipedia-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikipedia/refs/heads/main/openapi/wikipedia-snapshots-api-openapi.yml
- filename: wikipedia-structured-contents-api-openapi.yml
  format: yaml
  label: Wikipedia / MediaWiki structured-contents API
  slug: wikipedia-structured-contents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikipedia/refs/heads/main/openapi/wikipedia-structured-contents-api-openapi.yml
- filename: wikipedia-structured-snapshots-api-openapi.yml
  format: yaml
  label: Wikipedia / MediaWiki structured-snapshots API
  slug: wikipedia-structured-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikipedia/refs/heads/main/openapi/wikipedia-structured-snapshots-api-openapi.yml
- filename: wikipedia-talk-pages-api-openapi.yml
  format: yaml
  label: Wikipedia / MediaWiki Talk pages API
  slug: wikipedia-talk-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikipedia/refs/heads/main/openapi/wikipedia-talk-pages-api-openapi.yml
- filename: wikipedia-transforms-api-openapi.yml
  format: yaml
  label: Wikipedia / MediaWiki Transforms API
  slug: wikipedia-transforms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikipedia/refs/heads/main/openapi/wikipedia-transforms-api-openapi.yml
- filename: wikipedia-wikidata-api-openapi.yml
  format: yaml
  label: Wikipedia / MediaWiki wikidata API
  slug: wikipedia-wikidata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikipedia/refs/heads/main/openapi/wikipedia-wikidata-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Wikipedia Authentication
name_suffix: Authentication
oauth_flows: []
overview: Wikipedia / MediaWiki secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Wikipedia / MediaWiki
provider_slug: wikipedia
scheme_count: 2
schemes:
- description: OAuth 2.0 bearer token from meta.wikimedia.org
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/wikipedia-mediawiki-action-api-openapi.yaml
  - openapi/wikipedia-mediawiki-core-rest-openapi.yaml
  - openapi/wikipedia-wikimedia-enterprise-openapi.yaml
  type: http
- description: Session cookie obtained via action=login or action=clientlogin
  in: cookie
  name: CookieAuth
  parameter: '{wiki}wikiUserID'
  sources:
  - openapi/wikipedia-mediawiki-action-api-openapi.yaml
  type: apiKey
slug: wikipedia-authentication
source_filename: wikipedia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/wikipedia-mediawiki-action-api-openapi.yaml, openapi/wikipedia-mediawiki-core-rest-openapi.yaml,\n  openapi/wikipedia-wikimedia-enterprise-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 bearer token from meta.wikimedia.org\n  sources:\n  - openapi/wikipedia-mediawiki-action-api-openapi.yaml\n  - openapi/wikipedia-mediawiki-core-rest-openapi.yaml\n  - openapi/wikipedia-wikimedia-enterprise-openapi.yaml\n- name: CookieAuth\n  type: apiKey\n  in: cookie\n  parameter: '{wiki}wikiUserID'\n  description: Session cookie obtained via action=login or action=clientlogin\n  sources:\n  - openapi/wikipedia-mediawiki-action-api-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wikipedia/refs/heads/main/authentication/wikipedia-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Open Data
- Public APIs
- Open Knowledge
- Encyclopedia
- Knowledge Graph
- Open-Source
- Non-Profit
---

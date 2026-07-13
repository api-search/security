---
api_key_in:
- cookie
api_specs:
- filename: wikipedia-mediawiki-action-api-openapi.yaml
  format: yaml
  label: MediaWiki Action API
  slug: mediawiki-action-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikipedia/refs/heads/main/openapi/wikipedia-mediawiki-action-api-openapi.yaml
- filename: wikipedia-mediawiki-core-rest-openapi.yaml
  format: yaml
  label: MediaWiki Core REST API
  slug: mediawiki-core-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikipedia/refs/heads/main/openapi/wikipedia-mediawiki-core-rest-openapi.yaml
- filename: wikipedia-rest-v1-openapi.yaml
  format: yaml
  label: Wikimedia REST API v1
  slug: wikimedia-rest-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikipedia/refs/heads/main/openapi/wikipedia-rest-v1-openapi.yaml
- filename: wikipedia-wikidata-sparql-openapi.yaml
  format: yaml
  label: Wikidata Query Service (SPARQL)
  slug: wikidata-query-service-sparql
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikipedia/refs/heads/main/openapi/wikipedia-wikidata-sparql-openapi.yaml
- filename: wikipedia-wikimedia-enterprise-openapi.yaml
  format: yaml
  label: Wikimedia Enterprise API
  slug: wikimedia-enterprise-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikipedia/refs/heads/main/openapi/wikipedia-wikimedia-enterprise-openapi.yaml
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
- Open Source
- Non-Profit
---

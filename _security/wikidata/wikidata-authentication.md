---
api_key_in:
- cookie
api_specs:
- filename: wikidata-mediawiki-openapi.yml
  format: yaml
  label: Wikibase REST API
  slug: wikibase-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikidata/refs/heads/main/openapi/wikidata-mediawiki-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Wikidata Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Wikidata secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Wikidata
provider_slug: wikidata
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://www.mediawiki.org/w/index.php?title=Special:OAuth/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://www.mediawiki.org/w/index.php?title=Special:OAuth/token
  name: OAuth2
  sources:
  - openapi/wikidata-mediawiki-openapi.yml
  type: oauth2
- in: cookie
  name: MediaWikiSession
  parameter: wikidataSession
  sources:
  - openapi/wikidata-mediawiki-openapi.yml
  type: apiKey
slug: wikidata-authentication
source_filename: wikidata-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/wikidata-mediawiki-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - cookie\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.mediawiki.org/w/index.php?title=Special:OAuth/authorize\n    tokenUrl: https://www.mediawiki.org/w/index.php?title=Special:OAuth/token\n    scopes: 2\n  sources:\n  - openapi/wikidata-mediawiki-openapi.yml\n- name: MediaWikiSession\n  type: apiKey\n  in: cookie\n  parameter: wikidataSession\n  sources:\n  - openapi/wikidata-mediawiki-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wikidata/refs/heads/main/authentication/wikidata-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Knowledge Graph
- Linked Data
- Open Data
- Semantic Web
- SPARQL
- Wikipedia
---

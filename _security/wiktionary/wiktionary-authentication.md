---
api_key_in: []
api_specs:
- filename: wiktionary-definition-api-openapi.yml
  format: yaml
  label: Wiktionary Definition API
  slug: wiktionary-definition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wiktionary/refs/heads/main/openapi/wiktionary-definition-api-openapi.yml
- filename: wiktionary-expandtemplates-api-openapi.yml
  format: yaml
  label: Wiktionary ExpandTemplates API
  slug: wiktionary-expandtemplates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wiktionary/refs/heads/main/openapi/wiktionary-expandtemplates-api-openapi.yml
- filename: wiktionary-file-api-openapi.yml
  format: yaml
  label: Wiktionary File API
  slug: wiktionary-file-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wiktionary/refs/heads/main/openapi/wiktionary-file-api-openapi.yml
- filename: wiktionary-history-api-openapi.yml
  format: yaml
  label: Wiktionary History API
  slug: wiktionary-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wiktionary/refs/heads/main/openapi/wiktionary-history-api-openapi.yml
- filename: wiktionary-opensearch-api-openapi.yml
  format: yaml
  label: Wiktionary OpenSearch API
  slug: wiktionary-opensearch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wiktionary/refs/heads/main/openapi/wiktionary-opensearch-api-openapi.yml
- filename: wiktionary-page-api-openapi.yml
  format: yaml
  label: Wiktionary Page API
  slug: wiktionary-page-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wiktionary/refs/heads/main/openapi/wiktionary-page-api-openapi.yml
- filename: wiktionary-page-content-api-openapi.yml
  format: yaml
  label: Wiktionary Page Content API
  slug: wiktionary-page-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wiktionary/refs/heads/main/openapi/wiktionary-page-content-api-openapi.yml
- filename: wiktionary-parse-api-openapi.yml
  format: yaml
  label: Wiktionary Parse API
  slug: wiktionary-parse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wiktionary/refs/heads/main/openapi/wiktionary-parse-api-openapi.yml
- filename: wiktionary-query-api-openapi.yml
  format: yaml
  label: Wiktionary Query API
  slug: wiktionary-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wiktionary/refs/heads/main/openapi/wiktionary-query-api-openapi.yml
- filename: wiktionary-search-api-openapi.yml
  format: yaml
  label: Wiktionary Search API
  slug: wiktionary-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wiktionary/refs/heads/main/openapi/wiktionary-search-api-openapi.yml
- filename: wiktionary-transform-api-openapi.yml
  format: yaml
  label: Wiktionary Transform API
  slug: wiktionary-transform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wiktionary/refs/heads/main/openapi/wiktionary-transform-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Wiktionary Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Wiktionary secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Wiktionary
provider_slug: wiktionary
scheme_count: 2
schemes:
- description: OAuth 2.0 access tokens issued via api.wikimedia.org.
  flows:
  - authorizationUrl: https://meta.wikimedia.org/w/rest.php/oauth2/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://meta.wikimedia.org/w/rest.php/oauth2/access_token
  name: oauth2
  sources:
  - openapi/wiktionary-core-rest-api-openapi-original.yml
  - openapi/wiktionary-mediawiki-action-api-openapi-original.yml
  type: oauth2
- description: Legacy BotPassword scoped credentials.
  name: botPassword
  scheme: basic
  sources:
  - openapi/wiktionary-mediawiki-action-api-openapi-original.yml
  type: http
slug: wiktionary-authentication
source_filename: wiktionary-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/wiktionary-core-rest-api-openapi-original.yml, openapi/wiktionary-mediawiki-action-api-openapi-original.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://meta.wikimedia.org/w/rest.php/oauth2/authorize\n    tokenUrl: https://meta.wikimedia.org/w/rest.php/oauth2/access_token\n    scopes: 1\n  description: OAuth 2.0 access tokens issued via api.wikimedia.org.\n  sources:\n  - openapi/wiktionary-core-rest-api-openapi-original.yml\n  - openapi/wiktionary-mediawiki-action-api-openapi-original.yml\n- name: botPassword\n  type: http\n  scheme: basic\n  description: Legacy BotPassword scoped credentials.\n  sources:\n  - openapi/wiktionary-mediawiki-action-api-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wiktionary/refs/heads/main/authentication/wiktionary-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Dictionaries
- Open Source
- Wikimedia
- MediaWiki
- Linguistics
- Open Data
- Public APIs
---

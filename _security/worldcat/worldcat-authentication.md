---
api_key_in:
- query
api_specs:
- filename: wcv2
  format: yaml
  label: WorldCat Search API
  slug: worldcat-search-api
  spec_type: OpenAPI
  url: https://developer.api.oclc.org/wcv2
- filename: wc-metadata-v2
  format: yaml
  label: WorldCat Metadata API
  slug: worldcat-metadata-api
  spec_type: OpenAPI
  url: https://developer.api.oclc.org/wc-metadata-v2
- filename: worldcat-knowledge-base-api.yml
  format: yaml
  label: WorldCat Knowledge Base API
  slug: worldcat-knowledge-base-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/worldcat/refs/heads/main/openapi/worldcat-knowledge-base-api.yml
- filename: entity-data
  format: yaml
  label: WorldCat Entities Data API
  slug: worldcat-entities-data-api
  spec_type: OpenAPI
  url: https://developer.api.oclc.org/entity-data
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Worldcat Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: WorldCat secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: WorldCat
provider_slug: worldcat
scheme_count: 2
schemes:
- flows:
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://oauth.oclc.org/token
  - authorizationUrl: https://oauth.oclc.org/auth
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://oauth.oclc.org/token
  name: entity_data_auth
  sources:
  - openapi/worldcat-entities-api.yml
  - openapi/worldcat-metadata-api.yml
  - openapi/worldcat-search-api.yml
  type: oauth2
- in: query
  name: api_key
  parameter: wskey
  sources:
  - openapi/worldcat-knowledge-base-api.yml
  type: apiKey
slug: worldcat-authentication
source_filename: worldcat-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/worldcat-entities-api.yml, openapi/worldcat-knowledge-base-api.yml, openapi/worldcat-metadata-api.yml,\n  openapi/worldcat-search-api.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - query\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: entity_data_auth\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://oauth.oclc.org/token\n    scopes: 2\n  - flow: authorizationCode\n    authorizationUrl: https://oauth.oclc.org/auth\n    tokenUrl: https://oauth.oclc.org/token\n    scopes: 2\n  sources:\n  - openapi/worldcat-entities-api.yml\n  - openapi/worldcat-metadata-api.yml\n  - openapi/worldcat-search-api.yml\n- name: api_key\n  type: apiKey\n  in: query\n  parameter: wskey\n  sources:\n  - openapi/worldcat-knowledge-base-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/worldcat/refs/heads/main/authentication/worldcat-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Libraries
- Bibliographic Records
- WorldCat
- OCLC
- Cataloging
- Metadata
- Discovery
- Books
- Media
- Linked Data
---

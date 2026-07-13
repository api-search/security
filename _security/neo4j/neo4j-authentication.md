---
api_key_in: []
api_specs:
- filename: neo4j-http-api-openapi.yml
  format: yaml
  label: Neo4j HTTP API
  slug: http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neo4j/refs/heads/main/openapi/neo4j-http-api-openapi.yml
- filename: neo4j-query-api-openapi.yml
  format: yaml
  label: Neo4j Query API
  slug: query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neo4j/refs/heads/main/openapi/neo4j-query-api-openapi.yml
- filename: neo4j-aura-api-openapi.yml
  format: yaml
  label: Neo4j Aura API
  slug: aura-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neo4j/refs/heads/main/openapi/neo4j-aura-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Neo4J Authentication
name_suffix: Authentication
oauth_flows: []
overview: Neo4j secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Neo4j
provider_slug: neo4j
scheme_count: 2
schemes:
- description: OAuth2 bearer token obtained from the /oauth/token endpoint using client credentials. Tokens expire after one hour.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/neo4j-aura-api-openapi.yml
  type: http
- description: HTTP Basic Authentication using the Neo4j database username and password encoded as a base64 hash.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/neo4j-http-api-openapi.yml
  type: http
slug: neo4j-authentication
source_filename: neo4j-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/neo4j-aura-api-openapi.yml, openapi/neo4j-http-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth2 bearer token obtained from the /oauth/token endpoint using client credentials.\n    Tokens expire after one hour.\n  sources:\n  - openapi/neo4j-aura-api-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication using the Neo4j database username and password encoded\n    as a base64 hash.\n  sources:\n  - openapi/neo4j-http-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/neo4j/refs/heads/main/authentication/neo4j-authentication.yml
summary_line: http · 2 schemes
tags:
- Graph Database
- Cypher
- Cloud
- GraphQL
- Drivers
- APIs
---

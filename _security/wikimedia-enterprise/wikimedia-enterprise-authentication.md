---
anonymous_access: false
api_key_in: []
api_specs:
- filename: wikimedia-enterprise-articles-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Articles API
  slug: wikimedia-enterprise-articles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wikimedia-enterprise/openapi/wikimedia-enterprise-articles-api-openapi.yml
- filename: wikimedia-enterprise-authentication-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Authentication API
  slug: wikimedia-enterprise-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wikimedia-enterprise/openapi/wikimedia-enterprise-authentication-api-openapi.yml
- filename: wikimedia-enterprise-batches-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Batches API
  slug: wikimedia-enterprise-batches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wikimedia-enterprise/openapi/wikimedia-enterprise-batches-api-openapi.yml
- filename: wikimedia-enterprise-codes-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Codes API
  slug: wikimedia-enterprise-codes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wikimedia-enterprise/openapi/wikimedia-enterprise-codes-api-openapi.yml
- filename: wikimedia-enterprise-languages-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Languages API
  slug: wikimedia-enterprise-languages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wikimedia-enterprise/openapi/wikimedia-enterprise-languages-api-openapi.yml
- filename: wikimedia-enterprise-namespaces-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Namespaces API
  slug: wikimedia-enterprise-namespaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wikimedia-enterprise/openapi/wikimedia-enterprise-namespaces-api-openapi.yml
- filename: wikimedia-enterprise-projects-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Projects API
  slug: wikimedia-enterprise-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wikimedia-enterprise/openapi/wikimedia-enterprise-projects-api-openapi.yml
- filename: wikimedia-enterprise-realtime-articles-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Realtime Articles API
  slug: wikimedia-enterprise-realtime-articles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wikimedia-enterprise/openapi/wikimedia-enterprise-realtime-articles-api-openapi.yml
- filename: wikimedia-enterprise-realtime-wikidata-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Realtime Wikidata API
  slug: wikimedia-enterprise-realtime-wikidata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wikimedia-enterprise/openapi/wikimedia-enterprise-realtime-wikidata-api-openapi.yml
- filename: wikimedia-enterprise-snapshots-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Snapshots API
  slug: wikimedia-enterprise-snapshots-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wikimedia-enterprise/openapi/wikimedia-enterprise-snapshots-api-openapi.yml
- filename: wikimedia-enterprise-structured-contents-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Structured Contents API
  slug: wikimedia-enterprise-structured-contents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wikimedia-enterprise/openapi/wikimedia-enterprise-structured-contents-api-openapi.yml
- filename: wikimedia-enterprise-structured-snapshots-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Structured Snapshots API
  slug: wikimedia-enterprise-structured-snapshots-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wikimedia-enterprise/openapi/wikimedia-enterprise-structured-snapshots-api-openapi.yml
- filename: wikimedia-enterprise-wikidata-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Wikidata API
  slug: wikimedia-enterprise-wikidata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wikimedia-enterprise/openapi/wikimedia-enterprise-wikidata-api-openapi.yml
- filename: wikimedia-enterprise-wikidata-batches-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Wikidata Batches API
  slug: wikimedia-enterprise-wikidata-batches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wikimedia-enterprise/openapi/wikimedia-enterprise-wikidata-batches-api-openapi.yml
- filename: wikimedia-enterprise-wikidata-snapshots-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Wikidata Snapshots API
  slug: wikimedia-enterprise-wikidata-snapshots-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wikimedia-enterprise/openapi/wikimedia-enterprise-wikidata-snapshots-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Wikimedia Enterprise Authentication
name_suffix: Authentication
oauth_flows: []
overview: Wikimedia Enterprise secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Wikimedia Enterprise
provider_slug: wikimedia-enterprise
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/wikimedia-enterprise-openapi.yml
  type: http
slug: wikimedia-enterprise-authentication
source_filename: wikimedia-enterprise-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: searched\nsource: https://enterprise.wikimedia.com/docs/authentication.md\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/wikimedia-enterprise-openapi.yml\ndocs: https://enterprise.wikimedia.com/docs/authentication/\ntoken_lifetimes:\n  access_token: 24 hours\n  id_token: 24 hours\n  refresh_token: 90 days or 90 refreshes, whichever comes first\nflow: POST /v1/login (username all lowercase + password) -> access, ID and refresh tokens; send access_token as Bearer; POST /v1/token-refresh before expiry; POST /v1/token-revoke to revoke. Access tokens can also be copied from the dashboard.\nauth_host: https://auth.enterprise.wikimedia.com\n"
source_yaml_url: https://artifacts.apis.io/wikimedia-enterprise/authentication/wikimedia-enterprise-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Wikipedia
- wikidata
- Open Knowledge
- Datasets
- Content
- Knowledge Graph
- Streaming
- AI Training Data
---

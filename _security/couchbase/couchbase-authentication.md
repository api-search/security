---
api_key_in:
- cookie
api_specs:
- filename: couchbase-server-rest-api-openapi.yml
  format: yaml
  label: Couchbase Server REST API
  slug: couchbase-server-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/couchbase/refs/heads/main/openapi/couchbase-server-rest-api-openapi.yml
- filename: couchbase-query-service-rest-api-openapi.yml
  format: yaml
  label: Couchbase Query Service REST API
  slug: couchbase-query-service-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/couchbase/refs/heads/main/openapi/couchbase-query-service-rest-api-openapi.yml
- filename: couchbase-analytics-service-rest-api-openapi.yml
  format: yaml
  label: Couchbase Analytics Service REST API
  slug: couchbase-analytics-service-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/couchbase/refs/heads/main/openapi/couchbase-analytics-service-rest-api-openapi.yml
- filename: couchbase-search-service-rest-api-openapi.yml
  format: yaml
  label: Couchbase Search Service REST API
  slug: couchbase-search-service-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/couchbase/refs/heads/main/openapi/couchbase-search-service-rest-api-openapi.yml
- filename: couchbase-eventing-service-rest-api-openapi.yml
  format: yaml
  label: Couchbase Eventing Service REST API
  slug: couchbase-eventing-service-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/couchbase/refs/heads/main/openapi/couchbase-eventing-service-rest-api-openapi.yml
- filename: couchbase-backup-service-rest-api-openapi.yml
  format: yaml
  label: Couchbase Backup Service REST API
  slug: couchbase-backup-service-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/couchbase/refs/heads/main/openapi/couchbase-backup-service-rest-api-openapi.yml
- filename: couchbase-xdcr-rest-api-openapi.yml
  format: yaml
  label: Couchbase XDCR REST API
  slug: couchbase-xdcr-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/couchbase/refs/heads/main/openapi/couchbase-xdcr-rest-api-openapi.yml
- filename: couchbase-capella-management-api-openapi.yml
  format: yaml
  label: Couchbase Capella Management API
  slug: couchbase-capella-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/couchbase/refs/heads/main/openapi/couchbase-capella-management-api-openapi.yml
- filename: couchbase-capella-app-services-public-api-openapi.yml
  format: yaml
  label: Couchbase Capella App Services Public API
  slug: couchbase-capella-app-services-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/couchbase/refs/heads/main/openapi/couchbase-capella-app-services-public-api-openapi.yml
- filename: couchbase-capella-app-services-admin-api-openapi.yml
  format: yaml
  label: Couchbase Capella App Services Admin API
  slug: couchbase-capella-app-services-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/couchbase/refs/heads/main/openapi/couchbase-capella-app-services-admin-api-openapi.yml
- filename: couchbase-sync-gateway-public-rest-api-openapi.yml
  format: yaml
  label: Couchbase Sync Gateway Public REST API
  slug: couchbase-sync-gateway-public-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/couchbase/refs/heads/main/openapi/couchbase-sync-gateway-public-rest-api-openapi.yml
- filename: couchbase-sync-gateway-admin-rest-api-openapi.yml
  format: yaml
  label: Couchbase Sync Gateway Admin REST API
  slug: couchbase-sync-gateway-admin-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/couchbase/refs/heads/main/openapi/couchbase-sync-gateway-admin-rest-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Couchbase Authentication
name_suffix: Authentication
oauth_flows: []
overview: Couchbase secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Couchbase
provider_slug: couchbase
scheme_count: 3
schemes:
- description: HTTP Basic Authentication using Couchbase Server credentials.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/couchbase-analytics-service-rest-api-openapi.yml
  - openapi/couchbase-backup-service-rest-api-openapi.yml
  - openapi/couchbase-capella-app-services-admin-api-openapi.yml
  - openapi/couchbase-capella-app-services-public-api-openapi.yml
  - openapi/couchbase-eventing-service-rest-api-openapi.yml
  - openapi/couchbase-query-service-rest-api-openapi.yml
  - openapi/couchbase-search-service-rest-api-openapi.yml
  - openapi/couchbase-server-rest-api-openapi.yml
  - openapi/couchbase-sync-gateway-admin-rest-api-openapi.yml
  - openapi/couchbase-sync-gateway-public-rest-api-openapi.yml
  - openapi/couchbase-xdcr-rest-api-openapi.yml
  type: http
- description: Session cookie authentication obtained from the _session endpoint.
  in: cookie
  name: sessionAuth
  parameter: SyncGatewaySession
  sources:
  - openapi/couchbase-capella-app-services-public-api-openapi.yml
  - openapi/couchbase-sync-gateway-public-rest-api-openapi.yml
  type: apiKey
- description: Bearer token authentication using a Capella API key secret.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/couchbase-capella-management-api-openapi.yml
  type: http
slug: couchbase-authentication
source_filename: couchbase-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/couchbase-analytics-service-rest-api-openapi.yml, openapi/couchbase-backup-service-rest-api-openapi.yml,\n  openapi/couchbase-capella-app-services-admin-api-openapi.yml, openapi/couchbase-capella-app-services-public-api-openapi.yml,\n  openapi/couchbase-capella-management-api-openapi.yml, openapi/couchbase-eventing-service-rest-api-openapi.yml,\n  openapi/couchbase-query-service-rest-api-openapi.yml, openapi/couchbase-search-service-rest-api-openapi.yml,\n  openapi/couchbase-server-rest-api-openapi.yml, openapi/couchbase-sync-gateway-admin-rest-api-openapi.yml,\n  openapi/couchbase-sync-gateway-public-rest-api-openapi.yml, openapi/couchbase-xdcr-rest-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication using Couchbase Server credentials.\n  sources:\n  - openapi/couchbase-analytics-service-rest-api-openapi.yml\n\
  \  - openapi/couchbase-backup-service-rest-api-openapi.yml\n  - openapi/couchbase-capella-app-services-admin-api-openapi.yml\n  - openapi/couchbase-capella-app-services-public-api-openapi.yml\n  - openapi/couchbase-eventing-service-rest-api-openapi.yml\n  - openapi/couchbase-query-service-rest-api-openapi.yml\n  - openapi/couchbase-search-service-rest-api-openapi.yml\n  - openapi/couchbase-server-rest-api-openapi.yml\n  - openapi/couchbase-sync-gateway-admin-rest-api-openapi.yml\n  - openapi/couchbase-sync-gateway-public-rest-api-openapi.yml\n  - openapi/couchbase-xdcr-rest-api-openapi.yml\n- name: sessionAuth\n  type: apiKey\n  in: cookie\n  parameter: SyncGatewaySession\n  description: Session cookie authentication obtained from the _session endpoint.\n  sources:\n  - openapi/couchbase-capella-app-services-public-api-openapi.yml\n  - openapi/couchbase-sync-gateway-public-rest-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token authentication\
  \ using a Capella API key secret.\n  sources:\n  - openapi/couchbase-capella-management-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/couchbase/refs/heads/main/authentication/couchbase-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Analytics
- App Services
- Backup
- Capella
- Cloud
- Database
- DBaaS
- Eventing
- Full-Text Search
- Gateway
- JSON
- Mobile
- NoSQL
- Replication
- SQL++
- Sync
- Vector Search
- XDCR
---

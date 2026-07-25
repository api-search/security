---
api_key_in: []
api_specs:
- filename: scylladb-account-api-openapi.yml
  format: yaml
  label: ScyllaDB Account API
  slug: scylladb-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scylladb/refs/heads/main/openapi/scylladb-account-api-openapi.yml
- filename: scylladb-account-cluster-network-api-openapi.yml
  format: yaml
  label: ScyllaDB Account Cluster Network API
  slug: scylladb-account-cluster-network-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scylladb/refs/heads/main/openapi/scylladb-account-cluster-network-api-openapi.yml
- filename: scylladb-account-network-cluster-connection-api-openapi.yml
  format: yaml
  label: ScyllaDB Account network cluster connection API
  slug: scylladb-account-network-cluster-connection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scylladb/refs/heads/main/openapi/scylladb-account-network-cluster-connection-api-openapi.yml
- filename: scylladb-cluster-api-openapi.yml
  format: yaml
  label: ScyllaDB Cluster API
  slug: scylladb-cluster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scylladb/refs/heads/main/openapi/scylladb-cluster-api-openapi.yml
- filename: scylladb-cluster-request-api-openapi.yml
  format: yaml
  label: ScyllaDB Cluster Request API
  slug: scylladb-cluster-request-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scylladb/refs/heads/main/openapi/scylladb-cluster-request-api-openapi.yml
- filename: scylladb-deployment-api-openapi.yml
  format: yaml
  label: ScyllaDB Deployment API
  slug: scylladb-deployment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scylladb/refs/heads/main/openapi/scylladb-deployment-api-openapi.yml
- filename: scylladb-pricing-api-openapi.yml
  format: yaml
  label: ScyllaDB Pricing API
  slug: scylladb-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scylladb/refs/heads/main/openapi/scylladb-pricing-api-openapi.yml
- filename: scylladb-vectorsearch-api-openapi.yml
  format: yaml
  label: ScyllaDB VectorSearch API
  slug: scylladb-vectorsearch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scylladb/refs/heads/main/openapi/scylladb-vectorsearch-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Scylladb Authentication
name_suffix: Authentication
oauth_flows: []
overview: ScyllaDB secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ScyllaDB
provider_slug: scylladb
scheme_count: 1
schemes:
- description: 'Authorization header, required in all authenticated requests.


    Header format: **Authorization: Bearer <token>**'
  name: Authorization
  scheme: bearer
  sources:
  - openapi/scylladb-cloud-management-api-openapi.yml
  type: http
slug: scylladb-authentication
source_filename: scylladb-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/scylladb-cloud-management-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: Authorization\n  type: http\n  scheme: bearer\n  description: |-\n    Authorization header, required in all authenticated requests.\n\n    Header format: **Authorization: Bearer <token>**\n  sources:\n  - openapi/scylladb-cloud-management-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scylladb/refs/heads/main/authentication/scylladb-authentication.yml
summary_line: http · 1 scheme
tags:
- Database
- NoSQL
- Cassandra Compatible
- DynamoDB Compatible
- Distributed Database
- Real-Time
- Vector Search
- Cloud Database
---

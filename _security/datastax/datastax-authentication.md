---
api_key_in: []
api_specs:
- filename: datastax-access-list-api-openapi.yml
  format: yaml
  label: DataStax Access List API
  slug: datastax-access-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datastax/refs/heads/main/openapi/datastax-access-list-api-openapi.yml
- filename: datastax-authentication-api-openapi.yml
  format: yaml
  label: DataStax Authentication API
  slug: datastax-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datastax/refs/heads/main/openapi/datastax-authentication-api-openapi.yml
- filename: datastax-clone-api-openapi.yml
  format: yaml
  label: DataStax Clone API
  slug: datastax-clone-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datastax/refs/heads/main/openapi/datastax-clone-api-openapi.yml
- filename: datastax-customer-keys-api-openapi.yml
  format: yaml
  label: DataStax Customer Keys API
  slug: datastax-customer-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datastax/refs/heads/main/openapi/datastax-customer-keys-api-openapi.yml
- filename: datastax-database-operations-api-openapi.yml
  format: yaml
  label: DataStax Database Operations API
  slug: datastax-database-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datastax/refs/heads/main/openapi/datastax-database-operations-api-openapi.yml
- filename: datastax-devops-access-list-api-openapi.yml
  format: yaml
  label: DataStax DevOps Access List API
  slug: datastax-devops-access-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datastax/refs/heads/main/openapi/datastax-devops-access-list-api-openapi.yml
- filename: datastax-enterprise-operations-api-openapi.yml
  format: yaml
  label: DataStax Enterprise Operations API
  slug: datastax-enterprise-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datastax/refs/heads/main/openapi/datastax-enterprise-operations-api-openapi.yml
- filename: datastax-migrations-api-openapi.yml
  format: yaml
  label: DataStax Migrations API
  slug: datastax-migrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datastax/refs/heads/main/openapi/datastax-migrations-api-openapi.yml
- filename: datastax-organization-operations-api-openapi.yml
  format: yaml
  label: DataStax Organization Operations API
  slug: datastax-organization-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datastax/refs/heads/main/openapi/datastax-organization-operations-api-openapi.yml
- filename: datastax-pcu-api-openapi.yml
  format: yaml
  label: DataStax PCU API
  slug: datastax-pcu-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datastax/refs/heads/main/openapi/datastax-pcu-api-openapi.yml
- filename: datastax-private-link-api-openapi.yml
  format: yaml
  label: DataStax Private Link API
  slug: datastax-private-link-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datastax/refs/heads/main/openapi/datastax-private-link-api-openapi.yml
- filename: datastax-regions-api-openapi.yml
  format: yaml
  label: DataStax Regions API
  slug: datastax-regions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datastax/refs/heads/main/openapi/datastax-regions-api-openapi.yml
- filename: datastax-roles-api-openapi.yml
  format: yaml
  label: DataStax Roles API
  slug: datastax-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datastax/refs/heads/main/openapi/datastax-roles-api-openapi.yml
- filename: datastax-scim-api-openapi.yml
  format: yaml
  label: DataStax SCIM API
  slug: datastax-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datastax/refs/heads/main/openapi/datastax-scim-api-openapi.yml
- filename: datastax-token-api-openapi.yml
  format: yaml
  label: DataStax Token API
  slug: datastax-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datastax/refs/heads/main/openapi/datastax-token-api-openapi.yml
- filename: datastax-users-api-openapi.yml
  format: yaml
  label: DataStax Users API
  slug: datastax-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datastax/refs/heads/main/openapi/datastax-users-api-openapi.yml
- filename: datastax-vpc-peering-api-openapi.yml
  format: yaml
  label: DataStax VPC Peering API
  slug: datastax-vpc-peering-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datastax/refs/heads/main/openapi/datastax-vpc-peering-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Datastax Authentication
name_suffix: Authentication
oauth_flows: []
overview: DataStax secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DataStax
provider_slug: datastax
scheme_count: 1
schemes:
- description: An application token must be passed in header in order to access the API. https://docs.datastax.com/en/astra-db-serverless/administration/manage-application-tokens.html
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/datastax-devops-openapi.json
  type: http
slug: datastax-authentication
source_filename: datastax-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/datastax-devops-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: An application token must be passed in header in order to access the API. https://docs.datastax.com/en/astra-db-serverless/administration/manage-application-tokens.html\n  sources:\n  - openapi/datastax-devops-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datastax/refs/heads/main/authentication/datastax-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Enterprise
- Database
- Vector Database
- Cassandra
- Artificial Intelligence
- RAG
- Serverless
- Streaming
- Developer Tools
---

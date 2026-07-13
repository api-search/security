---
api_key_in: []
api_specs:
- filename: rest-catalog-open-api.yaml
  format: yaml
  label: Apache Iceberg REST Catalog API
  slug: apache-iceberg-rest-catalog
  spec_type: OpenAPI
  url: https://github.com/apache/iceberg/blob/main/open-api/rest-catalog-open-api.yaml
- filename: all.yaml
  format: yaml
  label: Unity Catalog
  slug: unity-catalog
  spec_type: OpenAPI
  url: https://github.com/unitycatalog/unitycatalog/blob/main/api/all.yaml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Table Format Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Table Format secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Table Format
provider_slug: table-format
scheme_count: 2
schemes:
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/apache-iceberg-rest-catalog-openapi.yml
  type: http
- flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: /v1/oauth/tokens
  name: OAuth2
  sources:
  - openapi/apache-iceberg-rest-catalog-openapi.yml
  type: oauth2
slug: table-format-authentication
source_filename: table-format-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/apache-iceberg-rest-catalog-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/apache-iceberg-rest-catalog-openapi.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /v1/oauth/tokens\n    scopes: 1\n  sources:\n  - openapi/apache-iceberg-rest-catalog-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/table-format/refs/heads/main/authentication/table-format-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Data Lakehouse
- Open Table Format
- Apache Iceberg
- Delta Lake
- Apache Hudi
- Data Lake
- ACID Transactions
- Schema Evolution
- Time Travel
---

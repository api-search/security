---
api_key_in: []
api_specs:
- filename: soveren-assets-api-openapi.yml
  format: yaml
  label: Soveren Assets API
  slug: soveren-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soveren/refs/heads/main/openapi/soveren-assets-api-openapi.yml
- filename: soveren-data-types-api-openapi.yml
  format: yaml
  label: Soveren Data Types API
  slug: soveren-data-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soveren/refs/heads/main/openapi/soveren-data-types-api-openapi.yml
- filename: soveren-endpoints-api-openapi.yml
  format: yaml
  label: Soveren Endpoints API
  slug: soveren-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soveren/refs/heads/main/openapi/soveren-endpoints-api-openapi.yml
- filename: soveren-kafka-api-openapi.yml
  format: yaml
  label: Soveren Kafka API
  slug: soveren-kafka-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soveren/refs/heads/main/openapi/soveren-kafka-api-openapi.yml
- filename: soveren-s3-api-openapi.yml
  format: yaml
  label: Soveren S3 API
  slug: soveren-s3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soveren/refs/heads/main/openapi/soveren-s3-api-openapi.yml
- filename: soveren-sql-db-api-openapi.yml
  format: yaml
  label: Soveren SQL DB API
  slug: soveren-sql-db-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soveren/refs/heads/main/openapi/soveren-sql-db-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Soveren Authentication
name_suffix: Authentication
oauth_flows: []
overview: Soveren secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Soveren
provider_slug: soveren
scheme_count: 1
schemes:
- description: Bearer token generated in the Soveren app under Integrations - External API.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/soveren-object-api-openapi.yml
  type: http
slug: soveren-authentication
source_filename: soveren-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/soveren-object-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token generated in the Soveren app under Integrations - External API.\n  sources:\n  - openapi/soveren-object-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/soveren/refs/heads/main/authentication/soveren-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Infra Devtools
- Data Security
- DSPM
- DDR
- Data Privacy
- Kubernetes
- Compliance
- Security
---

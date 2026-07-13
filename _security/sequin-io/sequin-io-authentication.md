---
api_key_in: []
api_specs:
- filename: sequin-io-openapi.yml
  format: yaml
  label: Sequin Sink Consumers API
  slug: sequin-io-sink-consumers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequin-io/refs/heads/main/openapi/sequin-io-openapi.yml
- filename: sequin-io-openapi.yml
  format: yaml
  label: Sequin Postgres Databases API
  slug: sequin-io-postgres-databases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequin-io/refs/heads/main/openapi/sequin-io-openapi.yml
- filename: sequin-io-openapi.yml
  format: yaml
  label: Sequin HTTP Endpoints API
  slug: sequin-io-http-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequin-io/refs/heads/main/openapi/sequin-io-openapi.yml
- filename: sequin-io-openapi.yml
  format: yaml
  label: Sequin Backfills API
  slug: sequin-io-backfills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequin-io/refs/heads/main/openapi/sequin-io-openapi.yml
- filename: sequin-io-openapi.yml
  format: yaml
  label: Sequin Stream Pull API
  slug: sequin-io-stream-pull-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequin-io/refs/heads/main/openapi/sequin-io-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Sequin Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sequin secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sequin
provider_slug: sequin-io
scheme_count: 1
schemes:
- description: 'Bearer token found in the Sequin console under "Manage account". Passed as `Authorization: Bearer YOUR_API_TOKEN`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/sequin-io-openapi.yml
  type: http
slug: sequin-io-authentication
source_filename: sequin-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sequin-io-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Bearer token found in the Sequin console under \"Manage account\". Passed as `Authorization:\n    Bearer YOUR_API_TOKEN`.'\n  sources:\n  - openapi/sequin-io-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sequin-io/refs/heads/main/authentication/sequin-io-authentication.yml
summary_line: http · 1 scheme
tags:
- Change Data Capture
- CDC
- Postgres
- Streaming
- Open Source
- Data Pipeline
---

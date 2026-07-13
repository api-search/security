---
api_key_in: []
api_specs:
- filename: axiom-co-openapi.yml
  format: yaml
  label: Axiom Ingest API
  slug: axiom-co-ingest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axiom-co/refs/heads/main/openapi/axiom-co-openapi.yml
- filename: axiom-co-openapi.yml
  format: yaml
  label: Axiom Query API (APL)
  slug: axiom-co-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axiom-co/refs/heads/main/openapi/axiom-co-openapi.yml
- filename: axiom-co-openapi.yml
  format: yaml
  label: Axiom Datasets API
  slug: axiom-co-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axiom-co/refs/heads/main/openapi/axiom-co-openapi.yml
- filename: axiom-co-openapi.yml
  format: yaml
  label: Axiom Fields API
  slug: axiom-co-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axiom-co/refs/heads/main/openapi/axiom-co-openapi.yml
- filename: axiom-co-openapi.yml
  format: yaml
  label: Axiom Annotations API
  slug: axiom-co-annotations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axiom-co/refs/heads/main/openapi/axiom-co-openapi.yml
- filename: axiom-co-openapi.yml
  format: yaml
  label: Axiom Monitors API
  slug: axiom-co-monitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axiom-co/refs/heads/main/openapi/axiom-co-openapi.yml
- filename: axiom-co-openapi.yml
  format: yaml
  label: Axiom Notifiers API
  slug: axiom-co-notifiers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axiom-co/refs/heads/main/openapi/axiom-co-openapi.yml
- filename: axiom-co-openapi.yml
  format: yaml
  label: Axiom Dashboards API
  slug: axiom-co-dashboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axiom-co/refs/heads/main/openapi/axiom-co-openapi.yml
- filename: axiom-co-openapi.yml
  format: yaml
  label: Axiom Virtual Fields API
  slug: axiom-co-virtual-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axiom-co/refs/heads/main/openapi/axiom-co-openapi.yml
- filename: axiom-co-openapi.yml
  format: yaml
  label: Axiom Starred Queries API
  slug: axiom-co-starred-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axiom-co/refs/heads/main/openapi/axiom-co-openapi.yml
- filename: axiom-co-openapi.yml
  format: yaml
  label: Axiom API Tokens API
  slug: axiom-co-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axiom-co/refs/heads/main/openapi/axiom-co-openapi.yml
- filename: axiom-co-openapi.yml
  format: yaml
  label: Axiom Users API
  slug: axiom-co-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axiom-co/refs/heads/main/openapi/axiom-co-openapi.yml
- filename: axiom-co-openapi.yml
  format: yaml
  label: Axiom Organizations API
  slug: axiom-co-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axiom-co/refs/heads/main/openapi/axiom-co-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Axiom Co Authentication
name_suffix: Authentication
oauth_flows: []
overview: Axiom secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Axiom
provider_slug: axiom-co
scheme_count: 1
schemes:
- description: Bearer token authentication using an Axiom API token or Personal Access Token (PAT). PAT-authenticated requests must also send the x-axiom-org-id header.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/axiom-co-openapi.yml
  type: http
slug: axiom-co-authentication
source_filename: axiom-co-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/axiom-co-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token authentication using an Axiom API token or Personal Access Token\n    (PAT). PAT-authenticated requests must also send the x-axiom-org-id header.\n  sources:\n  - openapi/axiom-co-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/axiom-co/refs/heads/main/authentication/axiom-co-authentication.yml
summary_line: http · 1 scheme
tags:
- Observability
- Log Management
- Event Data
- Logs
- Tracing
- Analytics
- APL
---

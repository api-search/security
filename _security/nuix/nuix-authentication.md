---
api_key_in:
- header
api_specs:
- filename: nuix-nuix-core-engine-rest-api-openapi.yml
  format: yaml
  label: Nuix Core Engine REST API
  slug: nuix-core-engine-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuix/refs/heads/main/openapi/nuix-nuix-core-engine-rest-api-openapi.yml
- filename: nuix-case-api-openapi.yml
  format: yaml
  label: Nuix Case API
  slug: nuix-case-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuix/refs/heads/main/openapi/nuix-case-api-openapi.yml
- filename: nuix-collection-and-survey-api-openapi.yml
  format: yaml
  label: Nuix Collection and Survey API
  slug: nuix-collection-and-survey-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuix/refs/heads/main/openapi/nuix-collection-and-survey-api-openapi.yml
- filename: nuix-collection-configuration-api-openapi.yml
  format: yaml
  label: Nuix Collection Configuration API
  slug: nuix-collection-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuix/refs/heads/main/openapi/nuix-collection-configuration-api-openapi.yml
- filename: nuix-computer-api-openapi.yml
  format: yaml
  label: Nuix Computer API
  slug: nuix-computer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuix/refs/heads/main/openapi/nuix-computer-api-openapi.yml
- filename: nuix-computer-configuration-api-openapi.yml
  format: yaml
  label: Nuix Computer Configuration API
  slug: nuix-computer-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuix/refs/heads/main/openapi/nuix-computer-configuration-api-openapi.yml
- filename: nuix-custodian-api-openapi.yml
  format: yaml
  label: Nuix Custodian API
  slug: nuix-custodian-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuix/refs/heads/main/openapi/nuix-custodian-api-openapi.yml
- filename: nuix-group-api-openapi.yml
  format: yaml
  label: Nuix Group API
  slug: nuix-group-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuix/refs/heads/main/openapi/nuix-group-api-openapi.yml
- filename: nuix-job-api-openapi.yml
  format: yaml
  label: Nuix Job API
  slug: nuix-job-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuix/refs/heads/main/openapi/nuix-job-api-openapi.yml
- filename: nuix-log-api-openapi.yml
  format: yaml
  label: Nuix Log API
  slug: nuix-log-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuix/refs/heads/main/openapi/nuix-log-api-openapi.yml
- filename: nuix-target-api-openapi.yml
  format: yaml
  label: Nuix Target API
  slug: nuix-target-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuix/refs/heads/main/openapi/nuix-target-api-openapi.yml
- filename: nuix-utility-api-openapi.yml
  format: yaml
  label: Nuix Utility API
  slug: nuix-utility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuix/refs/heads/main/openapi/nuix-utility-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Nuix Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nuix secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Nuix
provider_slug: nuix
scheme_count: 3
schemes:
- in: header
  name: ApiKeyAuth
  parameter: nuix-auth-token
  sources:
  - openapi/nuix-nuix-core-engine-rest-api-openapi.yml
  type: apiKey
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/nuix-nuix-core-engine-rest-api-openapi.yml
  type: http
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/nuix-nuix-ecc-rest-api-openapi.yml
  type: http
slug: nuix-authentication
source_filename: nuix-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/nuix-nuix-core-engine-rest-api-openapi.yml, openapi/nuix-nuix-ecc-rest-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: nuix-auth-token\n  sources:\n  - openapi/nuix-nuix-core-engine-rest-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/nuix-nuix-core-engine-rest-api-openapi.yml\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/nuix-nuix-ecc-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nuix/refs/heads/main/authentication/nuix-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Forensics
- eDiscovery
- Investigations
- Compliance
- Data Processing
- Legal Technology
- Intelligence
---

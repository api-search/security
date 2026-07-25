---
api_key_in: []
api_specs:
- filename: endor-labs-authentication-api-openapi.yml
  format: yaml
  label: Endor Labs Authentication API
  slug: endor-labs-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/endor-labs/refs/heads/main/openapi/endor-labs-authentication-api-openapi.yml
- filename: endor-labs-findings-api-openapi.yml
  format: yaml
  label: Endor Labs Findings API
  slug: endor-labs-findings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/endor-labs/refs/heads/main/openapi/endor-labs-findings-api-openapi.yml
- filename: endor-labs-namespaces-api-openapi.yml
  format: yaml
  label: Endor Labs Namespaces API
  slug: endor-labs-namespaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/endor-labs/refs/heads/main/openapi/endor-labs-namespaces-api-openapi.yml
- filename: endor-labs-packages-api-openapi.yml
  format: yaml
  label: Endor Labs Packages API
  slug: endor-labs-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/endor-labs/refs/heads/main/openapi/endor-labs-packages-api-openapi.yml
- filename: endor-labs-policies-api-openapi.yml
  format: yaml
  label: Endor Labs Policies API
  slug: endor-labs-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/endor-labs/refs/heads/main/openapi/endor-labs-policies-api-openapi.yml
- filename: endor-labs-projects-api-openapi.yml
  format: yaml
  label: Endor Labs Projects API
  slug: endor-labs-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/endor-labs/refs/heads/main/openapi/endor-labs-projects-api-openapi.yml
- filename: endor-labs-scan-results-api-openapi.yml
  format: yaml
  label: Endor Labs Scan Results API
  slug: endor-labs-scan-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/endor-labs/refs/heads/main/openapi/endor-labs-scan-results-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Endor Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Endor Labs secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Endor Labs
provider_slug: endor-labs
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Bearer access token obtained from POST /v1/auth/api-key by exchanging an Endor Labs API key and secret.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/endor-labs-openapi.yml
  type: http
slug: endor-labs-authentication
source_filename: endor-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/endor-labs-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Bearer access token obtained from POST /v1/auth/api-key by exchanging an Endor\n    Labs API key and secret.\n  sources:\n  - openapi/endor-labs-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/endor-labs/refs/heads/main/authentication/endor-labs-authentication.yml
summary_line: http · 1 scheme
tags:
- Security
- Software Supply Chain
- SCA
- Reachability
- AppSec
- AI Security
---

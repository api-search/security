---
anonymous_access: false
api_key_in: []
api_specs:
- filename: reachsocial-dev-catalog-api-openapi.yml
  format: yaml
  label: ReachSocial Catalog API
  slug: reachsocial-dev-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/reachsocial-dev/openapi/reachsocial-dev-catalog-api-openapi.yml
- filename: reachsocial-dev-jobs-api-openapi.yml
  format: yaml
  label: ReachSocial Jobs API
  slug: reachsocial-dev-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/reachsocial-dev/openapi/reachsocial-dev-jobs-api-openapi.yml
- filename: reachsocial-dev-operations-api-openapi.yml
  format: yaml
  label: ReachSocial Operations API
  slug: reachsocial-dev-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/reachsocial-dev/openapi/reachsocial-dev-operations-api-openapi.yml
- filename: reachsocial-dev-owner-api-openapi.yml
  format: yaml
  label: ReachSocial Owner API
  slug: reachsocial-dev-owner-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/reachsocial-dev/openapi/reachsocial-dev-owner-api-openapi.yml
- filename: reachsocial-dev-payments-api-openapi.yml
  format: yaml
  label: ReachSocial Payments API
  slug: reachsocial-dev-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/reachsocial-dev/openapi/reachsocial-dev-payments-api-openapi.yml
- filename: reachsocial-dev-resolve-api-openapi.yml
  format: yaml
  label: ReachSocial Resolve API
  slug: reachsocial-dev-resolve-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/reachsocial-dev/openapi/reachsocial-dev-resolve-api-openapi.yml
- filename: reachsocial-dev-services-api-openapi.yml
  format: yaml
  label: ReachSocial Services API
  slug: reachsocial-dev-services-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/reachsocial-dev/openapi/reachsocial-dev-services-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: derived
name: ReachSocial Authentication
name_suffix: Authentication
oauth_flows: []
overview: ReachSocial declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: ReachSocial
provider_slug: reachsocial-dev
scheme_count: 4
schemes:
- description: Private ReachSocial B2B API key.
  id: bearerAuth
  scheme: bearer
  type: http
- description: x402 v2 payment signature after the initial 402 challenge.
  id: x402Payment
  in: header
  name: PAYMENT-SIGNATURE
  type: apiKey
- description: Opaque token returned once for an anonymous asynchronous job.
  id: jobToken
  in: header
  name: X-Job-Token
  type: apiKey
- description: Protected owner-operations token; never used by public agents.
  id: adminToken
  in: header
  name: X-Admin-Token
  type: apiKey
slug: reachsocial-dev-authentication
source_filename: reachsocial-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: derived\nsource: https://reachsocial.dev/openapi.json\nschemes:\n  - id: bearerAuth\n    type: http\n    scheme: bearer\n    description: \"Private ReachSocial B2B API key.\"\n  - id: x402Payment\n    type: apiKey\n    in: header\n    name: PAYMENT-SIGNATURE\n    description: \"x402 v2 payment signature after the initial 402 challenge.\"\n  - id: jobToken\n    type: apiKey\n    in: header\n    name: X-Job-Token\n    description: \"Opaque token returned once for an anonymous asynchronous job.\"\n  - id: adminToken\n    type: apiKey\n    in: header\n    name: X-Admin-Token\n    description: \"Protected owner-operations token; never used by public agents.\"\n"
source_yaml_url: https://artifacts.apis.io/reachsocial-dev/authentication/reachsocial-dev-authentication.yml
summary_line: 4 schemes
tags:
- Social
- Data
- Public
- Payments
---

---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: nohumans-directory-alerts-api-openapi.yml
  format: yaml
  label: nohumans.directory Alerts API
  slug: nohumans-directory-alerts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nohumans-directory/openapi/nohumans-directory-alerts-api-openapi.yml
- filename: nohumans-directory-attestations-api-openapi.yml
  format: yaml
  label: nohumans.directory Attestations API
  slug: nohumans-directory-attestations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nohumans-directory/openapi/nohumans-directory-attestations-api-openapi.yml
- filename: nohumans-directory-changes-api-openapi.yml
  format: yaml
  label: nohumans.directory Changes API
  slug: nohumans-directory-changes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nohumans-directory/openapi/nohumans-directory-changes-api-openapi.yml
- filename: nohumans-directory-check-api-openapi.yml
  format: yaml
  label: nohumans.directory Check API
  slug: nohumans-directory-check-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nohumans-directory/openapi/nohumans-directory-check-api-openapi.yml
- filename: nohumans-directory-demand-api-openapi.yml
  format: yaml
  label: nohumans.directory Demand API
  slug: nohumans-directory-demand-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nohumans-directory/openapi/nohumans-directory-demand-api-openapi.yml
- filename: nohumans-directory-discover-api-openapi.yml
  format: yaml
  label: nohumans.directory Discover API
  slug: nohumans-directory-discover-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nohumans-directory/openapi/nohumans-directory-discover-api-openapi.yml
- filename: nohumans-directory-listings-api-openapi.yml
  format: yaml
  label: nohumans.directory Listings API
  slug: nohumans-directory-listings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nohumans-directory/openapi/nohumans-directory-listings-api-openapi.yml
- filename: nohumans-directory-methodology-json-api-openapi.yml
  format: yaml
  label: nohumans.directory Methodology.json API
  slug: nohumans-directory-methodology-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nohumans-directory/openapi/nohumans-directory-methodology-json-api-openapi.yml
- filename: nohumans-directory-reports-api-openapi.yml
  format: yaml
  label: nohumans.directory Reports API
  slug: nohumans-directory-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nohumans-directory/openapi/nohumans-directory-reports-api-openapi.yml
- filename: nohumans-directory-resolve-api-openapi.yml
  format: yaml
  label: nohumans.directory Resolve API
  slug: nohumans-directory-resolve-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nohumans-directory/openapi/nohumans-directory-resolve-api-openapi.yml
- filename: nohumans-directory-sellers-api-openapi.yml
  format: yaml
  label: nohumans.directory Sellers API
  slug: nohumans-directory-sellers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nohumans-directory/openapi/nohumans-directory-sellers-api-openapi.yml
- filename: nohumans-directory-state-api-openapi.yml
  format: yaml
  label: nohumans.directory State API
  slug: nohumans-directory-state-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nohumans-directory/openapi/nohumans-directory-state-api-openapi.yml
- filename: nohumans-directory-state-json-api-openapi.yml
  format: yaml
  label: nohumans.directory State.json API
  slug: nohumans-directory-state-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nohumans-directory/openapi/nohumans-directory-state-json-api-openapi.yml
- filename: nohumans-directory-stats-api-openapi.yml
  format: yaml
  label: nohumans.directory Stats API
  slug: nohumans-directory-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nohumans-directory/openapi/nohumans-directory-stats-api-openapi.yml
- filename: nohumans-directory-verdicts-api-openapi.yml
  format: yaml
  label: nohumans.directory Verdicts API
  slug: nohumans-directory-verdicts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nohumans-directory/openapi/nohumans-directory-verdicts-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: nohumans.directory Authentication
name_suffix: Authentication
oauth_flows: []
overview: nohumans.directory secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: nohumans.directory
provider_slug: nohumans-directory
scheme_count: 2
schemes:
- description: Returned once at submission or via the claim flow; x-edit-token accepted as alias
  in: header
  name: claimToken
  parameter: x-claim-token
  sources:
  - openapi/nohumans-directory-openapi.json
  - openapi/openapi.json
  type: apiKey
- description: 'Same claim token as Authorization: Bearer'
  name: bearer
  scheme: bearer
  sources:
  - openapi/nohumans-directory-openapi.json
  - openapi/openapi.json
  type: http
slug: nohumans-directory-authentication
source_filename: nohumans-directory-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: derived\nsource: openapi/nohumans-directory-openapi.json, openapi/openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: claimToken\n  type: apiKey\n  in: header\n  parameter: x-claim-token\n  description: Returned once at submission or via the claim flow; x-edit-token accepted as alias\n  sources:\n  - openapi/nohumans-directory-openapi.json\n  - openapi/openapi.json\n- name: bearer\n  type: http\n  scheme: bearer\n  description: 'Same claim token as Authorization: Bearer'\n  sources:\n  - openapi/nohumans-directory-openapi.json\n  - openapi/openapi.json\n"
source_yaml_url: https://artifacts.apis.io/nohumans-directory/authentication/nohumans-directory-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Directory
- API Registry
- Paid API Verification
- AI Agents
- MCP Service
---

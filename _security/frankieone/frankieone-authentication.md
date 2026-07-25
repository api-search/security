---
api_key_in:
- header
api_specs:
- filename: frankieone-audit-api-openapi.yml
  format: yaml
  label: FrankieOne Audit API
  slug: frankieone-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frankieone/refs/heads/main/openapi/frankieone-audit-api-openapi.yml
- filename: frankieone-hostedurl-api-openapi.yml
  format: yaml
  label: FrankieOne HostedURL API
  slug: frankieone-hostedurl-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frankieone/refs/heads/main/openapi/frankieone-hostedurl-api-openapi.yml
- filename: frankieone-idv-api-openapi.yml
  format: yaml
  label: FrankieOne IDV API
  slug: frankieone-idv-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frankieone/refs/heads/main/openapi/frankieone-idv-api-openapi.yml
- filename: frankieone-individual-documents-api-openapi.yml
  format: yaml
  label: FrankieOne Individual Documents API
  slug: frankieone-individual-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frankieone/refs/heads/main/openapi/frankieone-individual-documents-api-openapi.yml
- filename: frankieone-individual-entities-api-openapi.yml
  format: yaml
  label: FrankieOne Individual Entities API
  slug: frankieone-individual-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frankieone/refs/heads/main/openapi/frankieone-individual-entities-api-openapi.yml
- filename: frankieone-individual-entity-elements-api-openapi.yml
  format: yaml
  label: FrankieOne Individual Entity Elements API
  slug: frankieone-individual-entity-elements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frankieone/refs/heads/main/openapi/frankieone-individual-entity-elements-api-openapi.yml
- filename: frankieone-individual-profiles-api-openapi.yml
  format: yaml
  label: FrankieOne Individual Profiles API
  slug: frankieone-individual-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frankieone/refs/heads/main/openapi/frankieone-individual-profiles-api-openapi.yml
- filename: frankieone-individual-results-api-openapi.yml
  format: yaml
  label: FrankieOne Individual Results API
  slug: frankieone-individual-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frankieone/refs/heads/main/openapi/frankieone-individual-results-api-openapi.yml
- filename: frankieone-individual-risks-api-openapi.yml
  format: yaml
  label: FrankieOne Individual Risks API
  slug: frankieone-individual-risks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frankieone/refs/heads/main/openapi/frankieone-individual-risks-api-openapi.yml
- filename: frankieone-individual-workflows-api-openapi.yml
  format: yaml
  label: FrankieOne Individual Workflows API
  slug: frankieone-individual-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frankieone/refs/heads/main/openapi/frankieone-individual-workflows-api-openapi.yml
- filename: frankieone-matchlists-api-openapi.yml
  format: yaml
  label: FrankieOne Matchlists API
  slug: frankieone-matchlists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frankieone/refs/heads/main/openapi/frankieone-matchlists-api-openapi.yml
- filename: frankieone-monitoring-api-openapi.yml
  format: yaml
  label: FrankieOne Monitoring API
  slug: frankieone-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frankieone/refs/heads/main/openapi/frankieone-monitoring-api-openapi.yml
- filename: frankieone-search-api-openapi.yml
  format: yaml
  label: FrankieOne Search API
  slug: frankieone-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frankieone/refs/heads/main/openapi/frankieone-search-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Frankieone Authentication
name_suffix: Authentication
oauth_flows: []
overview: FrankieOne secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: FrankieOne
provider_slug: frankieone
scheme_count: 2
schemes:
- in: header
  name: Api-Key
  parameter: api_key
  sources:
  - openapi/core-v2-openapi.yml
  - openapi/kyc-v2-openapi.json
  type: apiKey
- bearerFormat: JWT
  name: jwt
  scheme: bearer
  sources:
  - openapi/core-v2-openapi.yml
  - openapi/kyc-v2-openapi.json
  type: http
slug: frankieone-authentication
source_filename: frankieone-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/core-v2-openapi.yml, openapi/kyc-v2-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: Api-Key\n  type: apiKey\n  in: header\n  parameter: api_key\n  sources:\n  - openapi/core-v2-openapi.yml\n  - openapi/kyc-v2-openapi.json\n- name: jwt\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/core-v2-openapi.yml\n  - openapi/kyc-v2-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/frankieone/refs/heads/main/authentication/frankieone-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Identity Verification
- KYC
- KYB
- AML
- Fraud
- Compliance
---

---
api_key_in: []
api_specs:
- filename: taboola-accounts-api-openapi.yml
  format: yaml
  label: Taboola Accounts API
  slug: taboola-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-accounts-api-openapi.yml
- filename: taboola-audience-targeting-api-openapi.yml
  format: yaml
  label: Taboola Audience Targeting API
  slug: taboola-audience-targeting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-audience-targeting-api-openapi.yml
- filename: taboola-bulk-items-api-openapi.yml
  format: yaml
  label: Taboola Bulk Items API
  slug: taboola-bulk-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-bulk-items-api-openapi.yml
- filename: taboola-bulk-operations-api-openapi.yml
  format: yaml
  label: Taboola Bulk Operations API
  slug: taboola-bulk-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-bulk-operations-api-openapi.yml
- filename: taboola-campaign-items-api-openapi.yml
  format: yaml
  label: Taboola Campaign Items API
  slug: taboola-campaign-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-campaign-items-api-openapi.yml
- filename: taboola-campaigns-api-openapi.yml
  format: yaml
  label: Taboola Campaigns API
  slug: taboola-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-campaigns-api-openapi.yml
- filename: taboola-combined-audiences-api-openapi.yml
  format: yaml
  label: Taboola Combined Audiences API
  slug: taboola-combined-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-combined-audiences-api-openapi.yml
- filename: taboola-conversion-rules-api-openapi.yml
  format: yaml
  label: Taboola Conversion Rules API
  slug: taboola-conversion-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-conversion-rules-api-openapi.yml
- filename: taboola-custom-audiences-api-openapi.yml
  format: yaml
  label: Taboola Custom Audiences API
  slug: taboola-custom-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-custom-audiences-api-openapi.yml
- filename: taboola-dictionary-api-openapi.yml
  format: yaml
  label: Taboola Dictionary API
  slug: taboola-dictionary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-dictionary-api-openapi.yml
- filename: taboola-first-party-audiences-api-openapi.yml
  format: yaml
  label: Taboola First Party Audiences API
  slug: taboola-first-party-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-first-party-audiences-api-openapi.yml
- filename: taboola-lookalike-audiences-api-openapi.yml
  format: yaml
  label: Taboola Lookalike Audiences API
  slug: taboola-lookalike-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-lookalike-audiences-api-openapi.yml
- filename: taboola-marketplace-audiences-api-openapi.yml
  format: yaml
  label: Taboola Marketplace Audiences API
  slug: taboola-marketplace-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-marketplace-audiences-api-openapi.yml
- filename: taboola-reach-estimator-api-openapi.yml
  format: yaml
  label: Taboola Reach Estimator API
  slug: taboola-reach-estimator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-reach-estimator-api-openapi.yml
- filename: taboola-reports-api-openapi.yml
  format: yaml
  label: Taboola Reports API
  slug: taboola-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-reports-api-openapi.yml
- filename: taboola-video-items-api-openapi.yml
  format: yaml
  label: Taboola Video Items API
  slug: taboola-video-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-video-items-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Taboola Authentication
name_suffix: Authentication
oauth_flows: []
overview: Taboola secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Taboola
provider_slug: taboola
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/taboola-backstage-accounts-api-openapi.yml
  - openapi/taboola-backstage-audiences-api-openapi.yml
  - openapi/taboola-backstage-campaigns-api-openapi.yml
  - openapi/taboola-backstage-conversions-api-openapi.yml
  - openapi/taboola-backstage-dictionary-api-openapi.yml
  - openapi/taboola-backstage-items-api-openapi.yml
  - openapi/taboola-backstage-reports-api-openapi.yml
  type: http
slug: taboola-authentication
source_filename: taboola-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/taboola-backstage-accounts-api-openapi.yml, openapi/taboola-backstage-audiences-api-openapi.yml,\n  openapi/taboola-backstage-campaigns-api-openapi.yml, openapi/taboola-backstage-conversions-api-openapi.yml,\n  openapi/taboola-backstage-dictionary-api-openapi.yml, openapi/taboola-backstage-items-api-openapi.yml,\n  openapi/taboola-backstage-reports-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/taboola-backstage-accounts-api-openapi.yml\n  - openapi/taboola-backstage-audiences-api-openapi.yml\n  - openapi/taboola-backstage-campaigns-api-openapi.yml\n  - openapi/taboola-backstage-conversions-api-openapi.yml\n  - openapi/taboola-backstage-dictionary-api-openapi.yml\n  - openapi/taboola-backstage-items-api-openapi.yml\n  - openapi/taboola-backstage-reports-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/authentication/taboola-authentication.yml
summary_line: http · 1 scheme
tags:
- Advertising
- Native Advertising
- Discovery
- Performance Marketing
- AdTech
- Realize
- Backstage
- Recommendation
- Publisher
- Programmatic
---

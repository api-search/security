---
anonymous_access: false
api_key_in: []
api_specs:
- filename: audit-domains-account-api-openapi.yml
  format: yaml
  label: audit.domains Account API
  slug: audit-domains-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audit-domains/openapi/audit-domains-account-api-openapi.yml
- filename: audit-domains-appraisals-api-openapi.yml
  format: yaml
  label: audit.domains Appraisals API
  slug: audit-domains-appraisals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audit-domains/openapi/audit-domains-appraisals-api-openapi.yml
- filename: audit-domains-bulk-api-openapi.yml
  format: yaml
  label: audit.domains Bulk API
  slug: audit-domains-bulk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audit-domains/openapi/audit-domains-bulk-api-openapi.yml
- filename: audit-domains-machine-api-openapi.yml
  format: yaml
  label: audit.domains Machine API
  slug: audit-domains-machine-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audit-domains/openapi/audit-domains-machine-api-openapi.yml
- filename: audit-domains-sales-api-openapi.yml
  format: yaml
  label: audit.domains Sales API
  slug: audit-domains-sales-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audit-domains/openapi/audit-domains-sales-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Audit Domains Authentication
name_suffix: Authentication
oauth_flows: []
overview: audit.domains declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: audit.domains
provider_slug: audit-domains
scheme_count: 2
schemes:
- description: 'Authorization: Bearer ad_live_...

    '
  name: bearer
  type: http
- description: ''
  name: x-api-key
  type: apiKey
slug: audit-domains-authentication
source_filename: audit-domains-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: searched\nsource: https://audit.domains/developers/\nschemes:\n  - type: http\n    name: bearer\n    description: |\n      Authorization: Bearer ad_live_...\n  - type: apiKey\n    name: x-api-key\n    description: \"\"\n"
source_yaml_url: https://artifacts.apis.io/audit-domains/authentication/audit-domains-authentication.yml
summary_line: 2 schemes
tags:
- Domain
- Valuation
- Analytics
- Portfolio
---

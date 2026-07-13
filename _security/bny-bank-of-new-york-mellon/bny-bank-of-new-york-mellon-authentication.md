---
api_key_in: []
api_specs:
- filename: bny-asset-servicing-api-openapi.yml
  format: yaml
  label: BNY Asset Servicing API
  slug: asset-servicing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bny-bank-of-new-york-mellon/refs/heads/main/openapi/bny-asset-servicing-api-openapi.yml
- filename: bny-treasury-services-api-openapi.yml
  format: yaml
  label: BNY Treasury Services API
  slug: treasury-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bny-bank-of-new-york-mellon/refs/heads/main/openapi/bny-treasury-services-api-openapi.yml
- filename: bny-pershing-api-openapi.yml
  format: yaml
  label: BNY Pershing API
  slug: pershing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bny-bank-of-new-york-mellon/refs/heads/main/openapi/bny-pershing-api-openapi.yml
- filename: bny-markets-api-openapi.yml
  format: yaml
  label: BNY Markets API
  slug: markets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bny-bank-of-new-york-mellon/refs/heads/main/openapi/bny-markets-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Bny Bank Of New York Mellon Authentication
name_suffix: Authentication
oauth_flows: []
overview: BNY (Bank of New York Mellon) secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: BNY (Bank of New York Mellon)
provider_slug: bny-bank-of-new-york-mellon
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/bny-asset-servicing-api-openapi.yml
  - openapi/bny-markets-api-openapi.yml
  - openapi/bny-pershing-api-openapi.yml
  - openapi/bny-treasury-services-api-openapi.yml
  type: http
slug: bny-bank-of-new-york-mellon-authentication
source_filename: bny-bank-of-new-york-mellon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bny-asset-servicing-api-openapi.yml, openapi/bny-markets-api-openapi.yml, openapi/bny-pershing-api-openapi.yml,\n  openapi/bny-treasury-services-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/bny-asset-servicing-api-openapi.yml\n  - openapi/bny-markets-api-openapi.yml\n  - openapi/bny-pershing-api-openapi.yml\n  - openapi/bny-treasury-services-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bny-bank-of-new-york-mellon/refs/heads/main/authentication/bny-bank-of-new-york-mellon-authentication.yml
summary_line: http · 1 scheme
tags:
- Banking
- Custody
- Asset Servicing
- Treasury Services
- Payments
- Wealth Management
- Clearing
- Capital Markets
- Digital Assets
- Financial Services
---

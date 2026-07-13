---
api_key_in: []
api_specs:
- filename: kpler-openapi.yml
  format: yaml
  label: Kpler Liquids API
  slug: kpler-liquids-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kpler/refs/heads/main/openapi/kpler-openapi.yml
- filename: kpler-openapi.yml
  format: yaml
  label: Kpler LNG API
  slug: kpler-lng-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kpler/refs/heads/main/openapi/kpler-openapi.yml
- filename: kpler-openapi.yml
  format: yaml
  label: Kpler LPG API
  slug: kpler-lpg-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kpler/refs/heads/main/openapi/kpler-openapi.yml
- filename: kpler-openapi.yml
  format: yaml
  label: Kpler Dry Bulk API
  slug: kpler-dry-bulk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kpler/refs/heads/main/openapi/kpler-openapi.yml
- filename: kpler-openapi.yml
  format: yaml
  label: Kpler Freight API
  slug: kpler-freight-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kpler/refs/heads/main/openapi/kpler-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Kpler Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kpler secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Kpler
provider_slug: kpler
scheme_count: 2
schemes:
- description: Encoded Kpler client credentials in the Authorization header.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/kpler-openapi.yml
  type: http
- description: Token obtained from the /login endpoint.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/kpler-openapi.yml
  type: http
slug: kpler-authentication
source_filename: kpler-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/kpler-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Encoded Kpler client credentials in the Authorization header.\n  sources:\n  - openapi/kpler-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Token obtained from the /login endpoint.\n  sources:\n  - openapi/kpler-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kpler/refs/heads/main/authentication/kpler-authentication.yml
summary_line: http · 2 schemes
tags:
- Vessel Tracking
- Maritime
- Commodities
- Supply Chain
- AIS
- Trade Flows
- Shipping
- Energy
---

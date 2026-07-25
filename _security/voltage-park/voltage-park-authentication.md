---
api_key_in: []
api_specs:
- filename: voltage-park-bare-metal-api-openapi.yml
  format: yaml
  label: Voltage Park Bare Metal API
  slug: voltage-park-bare-metal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voltage-park/refs/heads/main/openapi/voltage-park-bare-metal-api-openapi.yml
- filename: voltage-park-billing-api-openapi.yml
  format: yaml
  label: Voltage Park Billing API
  slug: voltage-park-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voltage-park/refs/heads/main/openapi/voltage-park-billing-api-openapi.yml
- filename: voltage-park-locations-api-openapi.yml
  format: yaml
  label: Voltage Park Locations API
  slug: voltage-park-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voltage-park/refs/heads/main/openapi/voltage-park-locations-api-openapi.yml
- filename: voltage-park-organization-api-openapi.yml
  format: yaml
  label: Voltage Park Organization API
  slug: voltage-park-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voltage-park/refs/heads/main/openapi/voltage-park-organization-api-openapi.yml
- filename: voltage-park-storage-api-openapi.yml
  format: yaml
  label: Voltage Park Storage API
  slug: voltage-park-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voltage-park/refs/heads/main/openapi/voltage-park-storage-api-openapi.yml
- filename: voltage-park-validation-api-openapi.yml
  format: yaml
  label: Voltage Park Validation API
  slug: voltage-park-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voltage-park/refs/heads/main/openapi/voltage-park-validation-api-openapi.yml
- filename: voltage-park-virtual-machines-api-openapi.yml
  format: yaml
  label: Voltage Park Virtual Machines API
  slug: voltage-park-virtual-machines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voltage-park/refs/heads/main/openapi/voltage-park-virtual-machines-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Voltage Park Authentication
name_suffix: Authentication
oauth_flows: []
overview: Voltage Park secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Voltage Park
provider_slug: voltage-park
scheme_count: 1
schemes:
- description: Bearer API token created on the Developers page of the Voltage Park dashboard. Tokens are valid for one year before expiring.
  name: apiTokenAuth
  scheme: bearer
  sources:
  - openapi/voltage-park-openapi.yml
  type: http
slug: voltage-park-authentication
source_filename: voltage-park-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/voltage-park-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: apiTokenAuth\n  type: http\n  scheme: bearer\n  description: Bearer API token created on the Developers page of the Voltage Park dashboard.\n    Tokens are valid for one year before expiring.\n  sources:\n  - openapi/voltage-park-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voltage-park/refs/heads/main/authentication/voltage-park-authentication.yml
summary_line: http · 1 scheme
tags:
- GPU
- Cloud
- AI Infrastructure
- H100
- H200
- Bare Metal
---

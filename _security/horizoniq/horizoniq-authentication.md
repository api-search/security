---
api_key_in: []
api_specs:
- filename: horizoniq-action-items-api-openapi.yml
  format: yaml
  label: HorizonIQ Action Items API
  slug: horizoniq-action-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/horizoniq/refs/heads/main/openapi/horizoniq-action-items-api-openapi.yml
- filename: horizoniq-billing-api-openapi.yml
  format: yaml
  label: HorizonIQ Billing API
  slug: horizoniq-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/horizoniq/refs/heads/main/openapi/horizoniq-billing-api-openapi.yml
- filename: horizoniq-devices-api-openapi.yml
  format: yaml
  label: HorizonIQ Devices API
  slug: horizoniq-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/horizoniq/refs/heads/main/openapi/horizoniq-devices-api-openapi.yml
- filename: horizoniq-images-api-openapi.yml
  format: yaml
  label: HorizonIQ Images API
  slug: horizoniq-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/horizoniq/refs/heads/main/openapi/horizoniq-images-api-openapi.yml
- filename: horizoniq-managed-firewalls-api-openapi.yml
  format: yaml
  label: HorizonIQ Managed Firewalls API
  slug: horizoniq-managed-firewalls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/horizoniq/refs/heads/main/openapi/horizoniq-managed-firewalls-api-openapi.yml
- filename: horizoniq-servers-api-openapi.yml
  format: yaml
  label: HorizonIQ Servers API
  slug: horizoniq-servers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/horizoniq/refs/heads/main/openapi/horizoniq-servers-api-openapi.yml
- filename: horizoniq-ssl-certificates-api-openapi.yml
  format: yaml
  label: HorizonIQ SSL Certificates API
  slug: horizoniq-ssl-certificates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/horizoniq/refs/heads/main/openapi/horizoniq-ssl-certificates-api-openapi.yml
- filename: horizoniq-support-api-openapi.yml
  format: yaml
  label: HorizonIQ Support API
  slug: horizoniq-support-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/horizoniq/refs/heads/main/openapi/horizoniq-support-api-openapi.yml
- filename: horizoniq-user-accounts-api-openapi.yml
  format: yaml
  label: HorizonIQ User Accounts API
  slug: horizoniq-user-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/horizoniq/refs/heads/main/openapi/horizoniq-user-accounts-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Horizoniq Authentication
name_suffix: Authentication
oauth_flows: []
overview: HorizonIQ secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: HorizonIQ
provider_slug: horizoniq
scheme_count: 1
schemes:
- description: 'API token issued from the Compass portal (Profile > API Tokens). Sent as `Authorization: Bearer <token>`. See https://compass-horizoniq.readme.io/reference/authentication'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/horizoniq-compass-openapi-original.yml
  type: http
slug: horizoniq-authentication
source_filename: horizoniq-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/horizoniq-compass-openapi-original.yml + docs\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'API token issued from the Compass portal (Profile > API Tokens). Sent as `Authorization:\n    Bearer <token>`. See https://compass-horizoniq.readme.io/reference/authentication'\n  sources:\n  - openapi/horizoniq-compass-openapi-original.yml\ndocs: https://compass-horizoniq.readme.io/reference/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/horizoniq/refs/heads/main/authentication/horizoniq-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Enterprise
- Cloud
- Bare Metal
- Infrastructure
- Private Cloud
- Hosting
- Data-Center
- Compute
- Storage
---

---
api_key_in: []
api_specs:
- filename: hospitable-openapi.yml
  format: yaml
  label: Hospitable Properties API
  slug: hospitable-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hospitable/refs/heads/main/openapi/hospitable-openapi.yml
- filename: hospitable-openapi.yml
  format: yaml
  label: Hospitable Listings API
  slug: hospitable-listings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hospitable/refs/heads/main/openapi/hospitable-openapi.yml
- filename: hospitable-openapi.yml
  format: yaml
  label: Hospitable Reservations API
  slug: hospitable-reservations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hospitable/refs/heads/main/openapi/hospitable-openapi.yml
- filename: hospitable-openapi.yml
  format: yaml
  label: Hospitable Messages API
  slug: hospitable-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hospitable/refs/heads/main/openapi/hospitable-openapi.yml
- filename: hospitable-openapi.yml
  format: yaml
  label: Hospitable Calendar API
  slug: hospitable-calendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hospitable/refs/heads/main/openapi/hospitable-openapi.yml
- filename: hospitable-openapi.yml
  format: yaml
  label: Hospitable Reviews API
  slug: hospitable-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hospitable/refs/heads/main/openapi/hospitable-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Hospitable Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hospitable secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Hospitable
provider_slug: hospitable
scheme_count: 1
schemes:
- description: 'A Personal Access Token (PAT) or OAuth 2.0 access token supplied as `Authorization: Bearer <token>`. OAuth 2.0 authorization-code flow is used for vendor integrations; PATs are scoped to a single Hospitable account for personal use.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/hospitable-openapi.yml
  type: http
slug: hospitable-authentication
source_filename: hospitable-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hospitable-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'A Personal Access Token (PAT) or OAuth 2.0 access token supplied as `Authorization:\n    Bearer <token>`. OAuth 2.0 authorization-code flow is used for vendor integrations; PATs\n    are scoped to a single Hospitable account for personal use.'\n  sources:\n  - openapi/hospitable-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hospitable/refs/heads/main/authentication/hospitable-authentication.yml
summary_line: http · 1 scheme
tags:
- Vacation Rental
- Short-Term Rental
- Property Management
- Airbnb
- Hospitality
- Automation
---

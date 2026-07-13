---
api_key_in: []
api_specs:
- filename: gigsky-openapi.yml
  format: yaml
  label: GigSky Plans & Catalog API
  slug: gigsky-plans-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gigsky/refs/heads/main/openapi/gigsky-openapi.yml
- filename: gigsky-openapi.yml
  format: yaml
  label: GigSky eSIM Provisioning API
  slug: gigsky-esim-provisioning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gigsky/refs/heads/main/openapi/gigsky-openapi.yml
- filename: gigsky-openapi.yml
  format: yaml
  label: GigSky Orders API
  slug: gigsky-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gigsky/refs/heads/main/openapi/gigsky-openapi.yml
- filename: gigsky-openapi.yml
  format: yaml
  label: GigSky Usage API
  slug: gigsky-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gigsky/refs/heads/main/openapi/gigsky-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Gigsky Authentication
name_suffix: Authentication
oauth_flows: []
overview: GigSky secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: GigSky
provider_slug: gigsky
scheme_count: 1
schemes:
- description: Placeholder. GigSky does not publicly document its authentication scheme. Partner/enterprise credentials are issued during account-gated onboarding; the actual mechanism (API key, bearer token, OAuth, or mutual TLS) must be confirmed with GigSky directly.
  name: GigSkyPartnerAuth
  scheme: bearer
  sources:
  - openapi/gigsky-openapi.yml
  type: http
slug: gigsky-authentication
source_filename: gigsky-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/gigsky-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: GigSkyPartnerAuth\n  type: http\n  scheme: bearer\n  description: Placeholder. GigSky does not publicly document its authentication scheme. Partner/enterprise\n    credentials are issued during account-gated onboarding; the actual mechanism (API key, bearer\n    token, OAuth, or mutual TLS) must be confirmed with GigSky directly.\n  sources:\n  - openapi/gigsky-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gigsky/refs/heads/main/authentication/gigsky-authentication.yml
summary_line: http · 1 scheme
tags:
- eSIM
- Mobile Data
- Roaming
- Connectivity
- IoT
- Telecom
---

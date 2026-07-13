---
api_key_in: []
api_specs:
- filename: photon-health-openapi.yml
  format: yaml
  label: Photon Health Patients API
  slug: photon-health-patients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/photon-health/refs/heads/main/openapi/photon-health-openapi.yml
- filename: photon-health-openapi.yml
  format: yaml
  label: Photon Health Prescriptions API
  slug: photon-health-prescriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/photon-health/refs/heads/main/openapi/photon-health-openapi.yml
- filename: photon-health-openapi.yml
  format: yaml
  label: Photon Health Orders API
  slug: photon-health-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/photon-health/refs/heads/main/openapi/photon-health-openapi.yml
- filename: photon-health-openapi.yml
  format: yaml
  label: Photon Health Catalog & Medications API
  slug: photon-health-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/photon-health/refs/heads/main/openapi/photon-health-openapi.yml
- filename: photon-health-openapi.yml
  format: yaml
  label: Photon Health Pharmacies API
  slug: photon-health-pharmacies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/photon-health/refs/heads/main/openapi/photon-health-openapi.yml
- filename: photon-health-openapi.yml
  format: yaml
  label: Photon Health Webhooks API
  slug: photon-health-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/photon-health/refs/heads/main/openapi/photon-health-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Photon Health Authentication
name_suffix: Authentication
oauth_flows: []
overview: Photon Health secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Photon Health
provider_slug: photon-health
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: OAuth2 Bearer access token obtained through a client_credentials exchange (client_id, client_secret, audience, grant_type) against auth.photon.health.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/photon-health-openapi.yml
  type: http
slug: photon-health-authentication
source_filename: photon-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/photon-health-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth2 Bearer access token obtained through a client_credentials exchange (client_id,\n    client_secret, audience, grant_type) against auth.photon.health.\n  sources:\n  - openapi/photon-health-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/photon-health/refs/heads/main/authentication/photon-health-authentication.yml
summary_line: http · 1 scheme
tags:
- Health
- e-Prescribing
- eRx
- Prescriptions
- Pharmacy
- GraphQL
---

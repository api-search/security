---
api_key_in: []
api_specs:
- filename: iec-cim-customers-api-openapi.yml
  format: yaml
  label: iec-cim Customers API
  slug: iec-cim-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iec-cim/refs/heads/main/openapi/iec-cim-customers-api-openapi.yml
- filename: iec-cim-metering-api-openapi.yml
  format: yaml
  label: iec-cim Metering API
  slug: iec-cim-metering-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iec-cim/refs/heads/main/openapi/iec-cim-metering-api-openapi.yml
- filename: iec-cim-network-assets-api-openapi.yml
  format: yaml
  label: iec-cim Network Assets API
  slug: iec-cim-network-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iec-cim/refs/heads/main/openapi/iec-cim-network-assets-api-openapi.yml
- filename: iec-cim-outages-api-openapi.yml
  format: yaml
  label: iec-cim Outages API
  slug: iec-cim-outages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iec-cim/refs/heads/main/openapi/iec-cim-outages-api-openapi.yml
- filename: iec-cim-work-orders-api-openapi.yml
  format: yaml
  label: iec-cim Work Orders API
  slug: iec-cim-work-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iec-cim/refs/heads/main/openapi/iec-cim-work-orders-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Iec Cim Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Iec Cim secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Iec Cim
provider_slug: iec-cim
scheme_count: 2
schemes:
- flows:
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://auth.utility.example.com/oauth/token
  name: OAuth2
  sources:
  - openapi/iec-cim-61968-distribution-openapi.yml
  type: oauth2
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/iec-cim-61968-distribution-openapi.yml
  type: http
slug: iec-cim-authentication
source_filename: iec-cim-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/iec-cim-61968-distribution-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.utility.example.com/oauth/token\n    scopes: 2\n  sources:\n  - openapi/iec-cim-61968-distribution-openapi.yml\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/iec-cim-61968-distribution-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iec-cim/refs/heads/main/authentication/iec-cim-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags: []
---

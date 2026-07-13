---
api_key_in: []
api_specs:
- filename: texas-instruments-store-openapi.yml
  format: yaml
  label: Texas Instruments Store API
  slug: ti-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/texas-instruments/refs/heads/main/openapi/texas-instruments-store-openapi.yml
- filename: texas-instruments-product-information-openapi.yml
  format: yaml
  label: Texas Instruments Product Information API
  slug: ti-product-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/texas-instruments/refs/heads/main/openapi/texas-instruments-product-information-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Texas Instruments Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Texas Instruments secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Texas Instruments
provider_slug: texas-instruments
scheme_count: 1
schemes:
- description: OAuth 2.0 client credentials flow. Obtain access token using client_id and client_secret from your myTI developer account.
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://transact.ti.com/v1/oauth/accesstoken
  name: OAuth2
  sources:
  - openapi/texas-instruments-product-information-openapi.yml
  - openapi/texas-instruments-store-openapi.yml
  type: oauth2
slug: texas-instruments-authentication
source_filename: texas-instruments-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/texas-instruments-product-information-openapi.yml, openapi/texas-instruments-store-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://transact.ti.com/v1/oauth/accesstoken\n    scopes: 0\n  description: OAuth 2.0 client credentials flow. Obtain access token using client_id and client_secret\n    from your myTI developer account.\n  sources:\n  - openapi/texas-instruments-product-information-openapi.yml\n  - openapi/texas-instruments-store-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/texas-instruments/refs/heads/main/authentication/texas-instruments-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Electronics
- Ordering
- Semiconductors
- Supply Chain
- Fortune 500
---

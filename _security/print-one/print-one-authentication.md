---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: print-one-address-api-openapi.yml
  format: yaml
  label: print-one Address API
  slug: print-one-address-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/print-one/openapi/print-one-address-api-openapi.yml
- filename: print-one-campaigns-api-openapi.yml
  format: yaml
  label: print-one Campaigns API
  slug: print-one-campaigns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/print-one/openapi/print-one-campaigns-api-openapi.yml
- filename: print-one-coupons-api-openapi.yml
  format: yaml
  label: print-one Coupons API
  slug: print-one-coupons-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/print-one/openapi/print-one-coupons-api-openapi.yml
- filename: print-one-design-previews-api-openapi.yml
  format: yaml
  label: print-one Design Previews API
  slug: print-one-design-previews-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/print-one/openapi/print-one-design-previews-api-openapi.yml
- filename: print-one-designs-api-openapi.yml
  format: yaml
  label: print-one Designs API
  slug: print-one-designs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/print-one/openapi/print-one-designs-api-openapi.yml
- filename: print-one-imports-api-openapi.yml
  format: yaml
  label: print-one Imports API
  slug: print-one-imports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/print-one/openapi/print-one-imports-api-openapi.yml
- filename: print-one-items-api-openapi.yml
  format: yaml
  label: print-one Items API
  slug: print-one-items-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/print-one/openapi/print-one-items-api-openapi.yml
- filename: print-one-mailings-api-openapi.yml
  format: yaml
  label: print-one Mailings API
  slug: print-one-mailings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/print-one/openapi/print-one-mailings-api-openapi.yml
- filename: print-one-webhooks-api-openapi.yml
  format: yaml
  label: print-one Webhooks API
  slug: print-one-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/print-one/openapi/print-one-webhooks-api-openapi.yml
- filename: print-one-webhook-events-api-openapi.yml
  format: yaml
  label: print-one Webhook Events API
  slug: print-one-webhook-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/print-one/openapi/print-one-webhook-events-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Print One Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: print-one secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: print-one
provider_slug: print-one
scheme_count: 2
schemes:
- in: header
  name: API Key
  parameter: x-api-key
  sources:
  - openapi/print-one-openapi.json
  type: apiKey
- flows:
  - authorizationUrl: https://api.print.one/v2/oauth/authorize
    flow: authorizationCode
    scopes: 30
    tokenUrl: https://api.print.one/v2/oauth/token
  name: Oauth2
  sources:
  - openapi/print-one-openapi.json
  type: oauth2
slug: print-one-authentication
source_filename: print-one-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: derived\nsource: openapi/print-one-openapi.json\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: API Key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/print-one-openapi.json\n- name: Oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.print.one/v2/oauth/authorize\n    tokenUrl: https://api.print.one/v2/oauth/token\n    scopes: 30\n  sources:\n  - openapi/print-one-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/print-one/authentication/print-one-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Postcards
- API
- Direct Mail
- Marketing
- Automation
---

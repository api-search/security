---
api_key_in: []
api_specs:
- filename: clickfunnels-contacts-api-openapi.yml
  format: yaml
  label: ClickFunnels Contacts API
  slug: clickfunnels-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickfunnels/refs/heads/main/openapi/clickfunnels-contacts-api-openapi.yml
- filename: clickfunnels-fulfillments-api-openapi.yml
  format: yaml
  label: ClickFunnels Fulfillments API
  slug: clickfunnels-fulfillments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickfunnels/refs/heads/main/openapi/clickfunnels-fulfillments-api-openapi.yml
- filename: clickfunnels-products-api-openapi.yml
  format: yaml
  label: ClickFunnels Products API
  slug: clickfunnels-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickfunnels/refs/heads/main/openapi/clickfunnels-products-api-openapi.yml
- filename: clickfunnels-teams-api-openapi.yml
  format: yaml
  label: ClickFunnels Teams API
  slug: clickfunnels-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickfunnels/refs/heads/main/openapi/clickfunnels-teams-api-openapi.yml
- filename: clickfunnels-workspaces-api-openapi.yml
  format: yaml
  label: ClickFunnels Workspaces API
  slug: clickfunnels-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickfunnels/refs/heads/main/openapi/clickfunnels-workspaces-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Clickfunnels Authentication
name_suffix: Authentication
oauth_flows: []
overview: ClickFunnels secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ClickFunnels
provider_slug: clickfunnels
scheme_count: 1
schemes:
- description: ClickFunnels 2.0 API access token issued per team.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/clickfunnels-openapi.yml
  type: http
slug: clickfunnels-authentication
source_filename: clickfunnels-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/clickfunnels-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: ClickFunnels 2.0 API access token issued per team.\n  sources:\n  - openapi/clickfunnels-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clickfunnels/refs/heads/main/authentication/clickfunnels-authentication.yml
summary_line: http · 1 scheme
tags:
- Sales Funnels
- Landing Pages
- E-commerce
- Marketing
- Checkout
- CRM
---

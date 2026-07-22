---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Shipper Authentication
name_suffix: Authentication
oauth_flows: []
overview: Shipper secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Shipper
provider_slug: shipper
scheme_count: 1
schemes:
- description: API key issued per merchant account, sent in the X-API-Key request header. Sandbox keys are obtained by registering a sandbox account at https://bos.sandbox.shipper.id and contacting Shipper (cs@shipper.id); production keys are provisioned by the Shipper team.
  in: header
  name: X-API-Key
  parameter_name: X-API-Key
  sources:
  - docs
  type: apiKey
slug: shipper-authentication
source_filename: shipper-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://logistics-docs.shipper.id/docs/integration-flow\ndocs: https://logistics-docs.shipper.id/docs/sign-up-for-shipper-api-integration\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  notes: >-\n    Single API-key authentication. The key is passed in the X-API-Key HTTP\n    request header on every call. Keys are environment-scoped (separate sandbox\n    and production keys). There is no OAuth / OpenID Connect surface, so no\n    scopes artifact applies.\nschemes:\n- name: X-API-Key\n  type: apiKey\n  in: header\n  parameter_name: X-API-Key\n  description: >-\n    API key issued per merchant account, sent in the X-API-Key request header.\n    Sandbox keys are obtained by registering a sandbox account at\n    https://bos.sandbox.shipper.id and contacting Shipper (cs@shipper.id);\n    production keys are provisioned by the Shipper team.\n  sources: [docs]\nenvironments:\n- name: sandbox\n  base_url:\
  \ https://merchant-api-sandbox.shipper.id\n  dashboard: https://bos.sandbox.shipper.id\n- name: production\n  base_url: https://merchant-api.shipper.id\nkey_provisioning:\n  steps:\n  - Register for a Sandbox account at https://bos.sandbox.shipper.id and verify it.\n  - Contact the Shipper team (cs@shipper.id) to be granted API-key access.\n  - Set the webhook URL in the dashboard (Menu API > Set Webhook) to receive status callbacks.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shipper/refs/heads/main/authentication/shipper-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Logistics
- Shipping
- Fulfillment
- Supply Chain
- E-commerce
- Last Mile Delivery
- Courier
- Indonesia
---

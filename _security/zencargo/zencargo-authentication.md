---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: documented
name: Zencargo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zencargo secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Zencargo
provider_slug: zencargo
scheme_count: 1
schemes:
- description: 'Zencargo uses HTTP Basic Authentication for its GraphQL API. Use the API Key''s ID (an auto-generated UUID) as the username and the API Key''s secret as the password. Join them with a single colon (keyId:secret), base64-encode the result, and send it as `Authorization: Basic <base64>`. API keys are generated per user in the Zencargo app under Profile Settings > API Keys (production keys at https://app.zencargo.com/dashboard/settings/api-keys); the secret is shown only once at creation. The API URL itself is customer-provisioned per tenant and environment (https://{accountReference}.api.{environment}.zencargo.com/graphql).'
  name: basicAuth
  scheme: basic
  sources:
  - https://api-docs.zencargo.com/authenticating/
  - https://api-docs.zencargo.com/generating_api_key/
  - https://api-docs.zencargo.com/requesting_api_url/
  type: http
slug: zencargo-authentication
source_filename: zencargo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: documented\nsource: https://api-docs.zencargo.com/authenticating/\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: >-\n    Zencargo uses HTTP Basic Authentication for its GraphQL API. Use the API\n    Key's ID (an auto-generated UUID) as the username and the API Key's secret\n    as the password. Join them with a single colon (keyId:secret), base64-encode\n    the result, and send it as `Authorization: Basic <base64>`. API keys are\n    generated per user in the Zencargo app under Profile Settings > API Keys\n    (production keys at https://app.zencargo.com/dashboard/settings/api-keys);\n    the secret is shown only once at creation. The API URL itself is\n    customer-provisioned per tenant and environment\n    (https://{accountReference}.api.{environment}.zencargo.com/graphql).\n  sources:\n  - https://api-docs.zencargo.com/authenticating/\n  - https://api-docs.zencargo.com/generating_api_key/\n\
  \  - https://api-docs.zencargo.com/requesting_api_url/\nwebhookVerification:\n  method: HMAC-SHA256\n  header: Zencargo-Hmac-SHA256\n  encoding: base64\n  description: >-\n    Outbound webhook requests include a base64-encoded Zencargo-Hmac-SHA256\n    header computed from the webhook's sign token (shown once at webhook\n    creation) and the request body. Recompute the HMAC digest and compare to\n    verify the request originated from Zencargo.\n  source: https://api-docs.zencargo.com/webhooks/\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zencargo/refs/heads/main/authentication/zencargo-authentication.yml
summary_line: http · 1 scheme
tags:
- Freight Forwarding
- Supply Chain
- Logistics
- Ocean Freight
- Shipment Tracking
- Bookings
- Supply Chain Visibility
- Freight
- SaaS
- GraphQL
---

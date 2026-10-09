---
anonymous_access: false
api_key_in: []
api_specs:
- filename: shipcloud-addresses-api-openapi.yml
  format: yaml
  label: shipcloud Addresses API
  slug: shipcloud-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipcloud/refs/heads/main/openapi/shipcloud-addresses-api-openapi.yml
- filename: shipcloud-carriers-api-openapi.yml
  format: yaml
  label: shipcloud Carriers API
  slug: shipcloud-carriers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipcloud/refs/heads/main/openapi/shipcloud-carriers-api-openapi.yml
- filename: shipcloud-default-returns-address-api-openapi.yml
  format: yaml
  label: shipcloud Default Returns Address API
  slug: shipcloud-default-returns-address-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipcloud/refs/heads/main/openapi/shipcloud-default-returns-address-api-openapi.yml
- filename: shipcloud-default-shipping-address-api-openapi.yml
  format: yaml
  label: shipcloud Default Shipping Address API
  slug: shipcloud-default-shipping-address-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipcloud/refs/heads/main/openapi/shipcloud-default-shipping-address-api-openapi.yml
- filename: shipcloud-invoice-address-api-openapi.yml
  format: yaml
  label: shipcloud Invoice Address API
  slug: shipcloud-invoice-address-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipcloud/refs/heads/main/openapi/shipcloud-invoice-address-api-openapi.yml
- filename: shipcloud-manifests-api-openapi.yml
  format: yaml
  label: shipcloud Manifests API
  slug: shipcloud-manifests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipcloud/refs/heads/main/openapi/shipcloud-manifests-api-openapi.yml
- filename: shipcloud-me-api-openapi.yml
  format: yaml
  label: shipcloud Me API
  slug: shipcloud-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipcloud/refs/heads/main/openapi/shipcloud-me-api-openapi.yml
- filename: shipcloud-orders-api-openapi.yml
  format: yaml
  label: shipcloud Orders API
  slug: shipcloud-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipcloud/refs/heads/main/openapi/shipcloud-orders-api-openapi.yml
- filename: shipcloud-pickup-dropoff-locations-api-openapi.yml
  format: yaml
  label: shipcloud Pickup Dropoff Locations API
  slug: shipcloud-pickup-dropoff-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipcloud/refs/heads/main/openapi/shipcloud-pickup-dropoff-locations-api-openapi.yml
- filename: shipcloud-pickup-requests-api-openapi.yml
  format: yaml
  label: shipcloud Pickup Requests API
  slug: shipcloud-pickup-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipcloud/refs/heads/main/openapi/shipcloud-pickup-requests-api-openapi.yml
- filename: shipcloud-shipment-quotes-api-openapi.yml
  format: yaml
  label: shipcloud Shipment Quotes API
  slug: shipcloud-shipment-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipcloud/refs/heads/main/openapi/shipcloud-shipment-quotes-api-openapi.yml
- filename: shipcloud-shipments-api-openapi.yml
  format: yaml
  label: shipcloud Shipments API
  slug: shipcloud-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipcloud/refs/heads/main/openapi/shipcloud-shipments-api-openapi.yml
- filename: shipcloud-trackers-api-openapi.yml
  format: yaml
  label: shipcloud Trackers API
  slug: shipcloud-trackers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipcloud/refs/heads/main/openapi/shipcloud-trackers-api-openapi.yml
- filename: shipcloud-webhooks-api-openapi.yml
  format: yaml
  label: shipcloud Webhooks API
  slug: shipcloud-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipcloud/refs/heads/main/openapi/shipcloud-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Shipcloud Authentication
name_suffix: Authentication
oauth_flows: []
overview: shipcloud secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: shipcloud
provider_slug: shipcloud
scheme_count: 1
schemes:
- credential: API key as Basic auth username, empty password
  description: 'Authentication to our API has to be done via HTTP Basic Auth . You''ll have to provide your API key as the basic auth username. You don''t have to provide a password. Be advised: The API key has to be Base64 encoded.'
  key_types:
  - sandbox
  - live
  name: basic_auth
  scheme: basic
  sources:
  - openapi/shipcloud-openapi.yml
  - https://developers.shipcloud.io/concepts/
  transport: all API requests must be made using HTTPS
  type: http
slug: shipcloud-authentication
source_filename: shipcloud-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: searched\nsource: https://developers.shipcloud.io/concepts/\ndocs: https://developers.shipcloud.io/concepts/\nsummary:\n  types:\n  - http\nschemes:\n- name: basic_auth\n  type: http\n  scheme: basic\n  description: \"Authentication to our API has to be done via HTTP Basic Auth . You'll have to provide your API key as the basic auth username. You don't have to provide a password. Be advised: The API key has to be Base64 encoded.\"\n  credential: API key as Basic auth username, empty password\n  key_types:\n  - sandbox\n  - live\n  transport: \"all API requests must be made using HTTPS\"\n  sources:\n  - openapi/shipcloud-openapi.yml\n  - https://developers.shipcloud.io/concepts/\noptional_headers:\n- name: Affiliate-ID\n  note: \"To make things easier for our support team we'd kindly ask you to send a custom header with every request you're making ... The headers key is Affiliate-ID .\"\n  source: https://developers.shipcloud.io/integrations/\n\
  webhook_auth:\n  note: Webhook receivers can be secured with basic authorization (username and optional password supplied when creating the webhook); added 2022-03-22 per the API changelog.\n  source: https://developers.shipcloud.io/concepts/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shipcloud/refs/heads/main/authentication/shipcloud-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Shipping
- Logistics
- Carriers
- Labels
- Tracking
- E-Commerce
---

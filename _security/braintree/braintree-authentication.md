---
api_key_in: []
api_specs:
- filename: braintree-webhooks-asyncapi.yml
  format: yaml
  label: Braintree Webhooks
  slug: webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/braintree/refs/heads/main/asyncapi/braintree-webhooks-asyncapi.yml
- filename: braintree-add-ons-api-openapi.yml
  format: yaml
  label: braintree Add-Ons API
  slug: braintree-add-ons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/braintree/refs/heads/main/openapi/braintree-add-ons-api-openapi.yml
- filename: braintree-client-tokens-api-openapi.yml
  format: yaml
  label: braintree Client Tokens API
  slug: braintree-client-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/braintree/refs/heads/main/openapi/braintree-client-tokens-api-openapi.yml
- filename: braintree-customers-api-openapi.yml
  format: yaml
  label: braintree Customers API
  slug: braintree-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/braintree/refs/heads/main/openapi/braintree-customers-api-openapi.yml
- filename: braintree-discounts-api-openapi.yml
  format: yaml
  label: braintree Discounts API
  slug: braintree-discounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/braintree/refs/heads/main/openapi/braintree-discounts-api-openapi.yml
- filename: braintree-disputes-api-openapi.yml
  format: yaml
  label: braintree Disputes API
  slug: braintree-disputes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/braintree/refs/heads/main/openapi/braintree-disputes-api-openapi.yml
- filename: braintree-payment-methods-api-openapi.yml
  format: yaml
  label: braintree Payment Methods API
  slug: braintree-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/braintree/refs/heads/main/openapi/braintree-payment-methods-api-openapi.yml
- filename: braintree-plans-api-openapi.yml
  format: yaml
  label: braintree Plans API
  slug: braintree-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/braintree/refs/heads/main/openapi/braintree-plans-api-openapi.yml
- filename: braintree-subscriptions-api-openapi.yml
  format: yaml
  label: braintree Subscriptions API
  slug: braintree-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/braintree/refs/heads/main/openapi/braintree-subscriptions-api-openapi.yml
- filename: braintree-transactions-api-openapi.yml
  format: yaml
  label: braintree Transactions API
  slug: braintree-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/braintree/refs/heads/main/openapi/braintree-transactions-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Braintree Authentication
name_suffix: Authentication
oauth_flows: []
overview: braintree secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: braintree
provider_slug: braintree
scheme_count: 1
schemes:
- description: HTTP Basic Authentication using the merchant's public API key as the username and private API key as the password, Base64-encoded per RFC 7617.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/braintree-payments-openapi.yml
  - openapi/braintree-subscriptions-openapi.yml
  type: http
slug: braintree-authentication
source_filename: braintree-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/braintree-payments-openapi.yml, openapi/braintree-subscriptions-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication using the merchant's public API key as the username\n    and private API key as the password, Base64-encoded per RFC 7617.\n  sources:\n  - openapi/braintree-payments-openapi.yml\n  - openapi/braintree-subscriptions-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/braintree/refs/heads/main/authentication/braintree-authentication.yml
summary_line: http · 1 scheme
tags: []
---

---
api_key_in: []
api_specs:
- filename: braintree-payments-openapi.yml
  format: yaml
  label: Braintree Payments API
  slug: payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/braintree/refs/heads/main/openapi/braintree-payments-openapi.yml
- filename: braintree-webhooks-asyncapi.yml
  format: yaml
  label: Braintree Webhooks
  slug: webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/braintree/refs/heads/main/asyncapi/braintree-webhooks-asyncapi.yml
- filename: braintree-payments-openapi.yml
  format: yaml
  label: Braintree Vault API
  slug: vault-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/braintree/refs/heads/main/openapi/braintree-payments-openapi.yml
- filename: braintree-subscriptions-openapi.yml
  format: yaml
  label: Braintree Subscriptions API
  slug: subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/braintree/refs/heads/main/openapi/braintree-subscriptions-openapi.yml
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

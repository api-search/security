---
api_key_in: []
api_specs:
- filename: western-union-balances-api-openapi.yml
  format: yaml
  label: western-union Balances API
  slug: western-union-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/western-union/refs/heads/main/openapi/western-union-balances-api-openapi.yml
- filename: western-union-batches-api-openapi.yml
  format: yaml
  label: western-union Batches API
  slug: western-union-batches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/western-union/refs/heads/main/openapi/western-union-batches-api-openapi.yml
- filename: western-union-customers-api-openapi.yml
  format: yaml
  label: western-union Customers API
  slug: western-union-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/western-union/refs/heads/main/openapi/western-union-customers-api-openapi.yml
- filename: western-union-health-api-openapi.yml
  format: yaml
  label: western-union Health API
  slug: western-union-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/western-union/refs/heads/main/openapi/western-union-health-api-openapi.yml
- filename: western-union-orders-api-openapi.yml
  format: yaml
  label: western-union Orders API
  slug: western-union-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/western-union/refs/heads/main/openapi/western-union-orders-api-openapi.yml
- filename: western-union-payments-api-openapi.yml
  format: yaml
  label: western-union Payments API
  slug: western-union-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/western-union/refs/heads/main/openapi/western-union-payments-api-openapi.yml
- filename: western-union-quotes-api-openapi.yml
  format: yaml
  label: western-union Quotes API
  slug: western-union-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/western-union/refs/heads/main/openapi/western-union-quotes-api-openapi.yml
auth_types:
- mutualTLS
description: ''
kind: authentication
layout: security
method: derived
name: Western Union Authentication
name_suffix: Authentication
oauth_flows: []
overview: western-union secures its APIs with mutualTLS across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: western-union
provider_slug: western-union
scheme_count: 1
schemes:
- description: Mutual TLS authentication using client certificates provided by Western Union upon enrollment in the Partnership Program. Include the certificate and key with every request.
  name: mtlsAuth
  sources:
  - openapi/western-union-mass-payments-openapi.yml
  type: mutualTLS
slug: western-union-authentication
source_filename: western-union-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/western-union-mass-payments-openapi.yml\nsummary:\n  types:\n  - mutualTLS\nschemes:\n- name: mtlsAuth\n  type: mutualTLS\n  description: Mutual TLS authentication using client certificates provided by Western Union\n    upon enrollment in the Partnership Program. Include the certificate and key with every request.\n  sources:\n  - openapi/western-union-mass-payments-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/western-union/refs/heads/main/authentication/western-union-authentication.yml
summary_line: mutualTLS · 1 scheme
tags:
- Fortune 500
---

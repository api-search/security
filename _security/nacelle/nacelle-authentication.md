---
anonymous_access: false
api_key_in: []
api_specs:
- filename: nacelle.postman_collection.json
  format: json
  label: Nacelle Storefront Products API
  slug: nacelle-storefront-products-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/collections/nacelle.postman_collection.json
- filename: nacelle.postman_collection.json
  format: json
  label: Nacelle Storefront Product Collections API
  slug: nacelle-storefront-product-collections-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/collections/nacelle.postman_collection.json
- filename: nacelle.postman_collection.json
  format: json
  label: Nacelle Storefront Content API
  slug: nacelle-storefront-content-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/collections/nacelle.postman_collection.json
- filename: nacelle.postman_collection.json
  format: json
  label: Nacelle Storefront Navigation and Spaces API
  slug: nacelle-storefront-navigation-spaces-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/collections/nacelle.postman_collection.json
- filename: nacelle.postman_collection.json
  format: json
  label: Nacelle Admin Indexing and Ingestion API
  slug: nacelle-admin-indexing-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/collections/nacelle.postman_collection.json
- filename: nacelle-addresses-api-openapi.yml
  format: yaml
  label: Nacelle Addresses API
  slug: nacelle-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/openapi/nacelle-addresses-api-openapi.yml
- filename: nacelle-checkout-api-openapi.yml
  format: yaml
  label: Nacelle Checkout API
  slug: nacelle-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/openapi/nacelle-checkout-api-openapi.yml
- filename: nacelle-credentials-api-openapi.yml
  format: yaml
  label: Nacelle Credentials API
  slug: nacelle-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/openapi/nacelle-credentials-api-openapi.yml
- filename: nacelle-customers-api-openapi.yml
  format: yaml
  label: Nacelle Customers API
  slug: nacelle-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/openapi/nacelle-customers-api-openapi.yml
- filename: nacelle-entries-alpha-api-openapi.yml
  format: yaml
  label: Nacelle entries (ALPHA) API
  slug: nacelle-entries-alpha-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/openapi/nacelle-entries-alpha-api-openapi.yml
- filename: nacelle-entries-api-openapi.yml
  format: yaml
  label: Nacelle Entries API
  slug: nacelle-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/openapi/nacelle-entries-api-openapi.yml
- filename: nacelle-entries-beta-api-openapi.yml
  format: yaml
  label: Nacelle entries (BETA) API
  slug: nacelle-entries-beta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/openapi/nacelle-entries-beta-api-openapi.yml
- filename: nacelle-fulfillments-api-openapi.yml
  format: yaml
  label: Nacelle Fulfillments API
  slug: nacelle-fulfillments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/openapi/nacelle-fulfillments-api-openapi.yml
- filename: nacelle-index-api-openapi.yml
  format: yaml
  label: Nacelle Index API
  slug: nacelle-index-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/openapi/nacelle-index-api-openapi.yml
- filename: nacelle-multiorders-api-openapi.yml
  format: yaml
  label: Nacelle Multiorders API
  slug: nacelle-multiorders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/openapi/nacelle-multiorders-api-openapi.yml
- filename: nacelle-orderitems-api-openapi.yml
  format: yaml
  label: Nacelle Orderitems API
  slug: nacelle-orderitems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/openapi/nacelle-orderitems-api-openapi.yml
- filename: nacelle-payment-api-openapi.yml
  format: yaml
  label: Nacelle Payment API
  slug: nacelle-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/openapi/nacelle-payment-api-openapi.yml
- filename: nacelle-paymentintent-api-openapi.yml
  format: yaml
  label: Nacelle Paymentintent API
  slug: nacelle-paymentintent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/openapi/nacelle-paymentintent-api-openapi.yml
- filename: nacelle-token-api-openapi.yml
  format: yaml
  label: Nacelle Token API
  slug: nacelle-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/openapi/nacelle-token-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Nacelle Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Nacelle secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Nacelle
provider_slug: nacelle
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://authimilate.api.nacelle.com/v1/token
  name: oauth2
  sources:
  - openapi/nacelle-auth-api-openapi.yml
  - openapi/nacelle-order-management-api-experimental-openapi.yml
  type: oauth2
slug: nacelle-authentication
source_filename: nacelle-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: derived\nsource: openapi/nacelle-auth-api-openapi.yml, openapi/nacelle-order-management-api-experimental-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://authimilate.api.nacelle.com/v1/token\n    scopes: 2\n  sources:\n  - openapi/nacelle-auth-api-openapi.yml\n  - openapi/nacelle-order-management-api-experimental-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/authentication/nacelle-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Commerce
- Headless Commerce
- Composable Commerce
- GraphQL
- Content
- Data Indexing
---

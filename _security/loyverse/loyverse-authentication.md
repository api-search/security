---
api_key_in: []
api_specs:
- filename: loyverse-openapi.yml
  format: yaml
  label: Loyverse Items API
  slug: loyverse-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loyverse/refs/heads/main/openapi/loyverse-openapi.yml
- filename: loyverse-openapi.yml
  format: yaml
  label: Loyverse Categories API
  slug: loyverse-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loyverse/refs/heads/main/openapi/loyverse-openapi.yml
- filename: loyverse-openapi.yml
  format: yaml
  label: Loyverse Receipts API
  slug: loyverse-receipts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loyverse/refs/heads/main/openapi/loyverse-openapi.yml
- filename: loyverse-openapi.yml
  format: yaml
  label: Loyverse Customers API
  slug: loyverse-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loyverse/refs/heads/main/openapi/loyverse-openapi.yml
- filename: loyverse-openapi.yml
  format: yaml
  label: Loyverse Inventory API
  slug: loyverse-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loyverse/refs/heads/main/openapi/loyverse-openapi.yml
- filename: loyverse-openapi.yml
  format: yaml
  label: Loyverse Stores API
  slug: loyverse-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loyverse/refs/heads/main/openapi/loyverse-openapi.yml
- filename: loyverse-openapi.yml
  format: yaml
  label: Loyverse Employees API
  slug: loyverse-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loyverse/refs/heads/main/openapi/loyverse-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Loyverse Authentication
name_suffix: Authentication
oauth_flows: []
overview: Loyverse secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Loyverse
provider_slug: loyverse
scheme_count: 2
schemes:
- description: 'Personal access token. Generated in the Loyverse Back Office under Settings, Access Tokens (up to 20 tokens per account, each with an optional expiration). A personal token grants unlimited access to all resources of the account that created it. Passed as `Authorization: Bearer [example key]`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - https://help.loyverse.com/help/loyverse-api
  - https://developer.loyverse.com/docs/
  type: http
- authorizationUrl: https://api.loyverse.com/oauth/authorize
  description: OAuth 2.0 authorization-code flow for third-party apps that act on behalf of other Loyverse merchants. Register an app in the Loyverse developer dashboard to obtain a client_id and client_secret, then request scoped permissions. Access is granted per scope rather than the unlimited access of a personal token.
  flow: authorizationCode
  name: oauth2
  scopes:
    CUSTOMERS_READ: Read customers and loyalty data.
    CUSTOMERS_WRITE: Create and update customers.
    EMPLOYEES_READ: Read employees.
    INVENTORY_READ: Read inventory levels.
    INVENTORY_WRITE: Update inventory levels.
    ITEMS_READ: Read items, categories, variants, modifiers, discounts, and taxes.
    ITEMS_WRITE: Create and update items and related catalog objects.
    MERCHANT_READ: Read merchant and store information.
    PAYMENT_TYPES_READ: Read payment types.
    RECEIPTS_READ: Read receipts (sales).
    RECEIPTS_WRITE: Create receipts.
    STORES_READ: Read stores.
  sources:
  - https://developer.loyverse.com/docs/
  - https://support.loyverse.com/en/articles/8061203-faqs-about-loyverse-api
  tokenUrl: https://api.loyverse.com/oauth/token
  type: oauth2
slug: loyverse-authentication
source_filename: loyverse-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/loyverse-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    Personal access token. Generated in the Loyverse Back Office under Settings,\n    Access Tokens (up to 20 tokens per account, each with an optional expiration).\n    A personal token grants unlimited access to all resources of the account that\n    created it. Passed as `Authorization: Bearer [example key]`.\n  sources:\n  - https://help.loyverse.com/help/loyverse-api\n  - https://developer.loyverse.com/docs/\n- name: oauth2\n  type: oauth2\n  flow: authorizationCode\n  authorizationUrl: https://api.loyverse.com/oauth/authorize\n  tokenUrl: https://api.loyverse.com/oauth/token\n  description: >-\n    OAuth 2.0 authorization-code flow for third-party apps that act on behalf of\n    other Loyverse merchants. Register an app in the Loyverse developer dashboard\n    to obtain\
  \ a client_id and client_secret, then request scoped permissions.\n    Access is granted per scope rather than the unlimited access of a personal\n    token.\n  scopes:\n    CUSTOMERS_READ: Read customers and loyalty data.\n    CUSTOMERS_WRITE: Create and update customers.\n    EMPLOYEES_READ: Read employees.\n    ITEMS_READ: Read items, categories, variants, modifiers, discounts, and taxes.\n    ITEMS_WRITE: Create and update items and related catalog objects.\n    INVENTORY_READ: Read inventory levels.\n    INVENTORY_WRITE: Update inventory levels.\n    MERCHANT_READ: Read merchant and store information.\n    PAYMENT_TYPES_READ: Read payment types.\n    RECEIPTS_READ: Read receipts (sales).\n    RECEIPTS_WRITE: Create receipts.\n    STORES_READ: Read stores.\n  sources:\n  - https://developer.loyverse.com/docs/\n  - https://support.loyverse.com/en/articles/8061203-faqs-about-loyverse-api\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loyverse/refs/heads/main/authentication/loyverse-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Point of Sale
- POS
- Retail
- Inventory
- Cafe and Restaurant
- Loyalty
- Payments
- Commerce
---

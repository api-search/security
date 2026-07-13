---
api_key_in: []
api_specs:
- filename: elastic-path-commerce-apis.zip
  format: yaml
  label: Elastic Path Commerce Cloud API
  slug: commerce-cloud-api
  spec_type: OpenAPI
  url: https://developer.elasticpath.com/elastic-path-commerce-apis.zip
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Elastic Path Authentication
name_suffix: Authentication
oauth_flows: []
overview: Elastic Path secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Elastic Path
provider_slug: elastic-path
scheme_count: 1
schemes:
- name: BearerToken
  scheme: bearer
  sources:
  - openapi/account-addresses.yaml
  - openapi/accounts.yaml
  - openapi/application-keys.yaml
  - openapi/carts.yaml
  - openapi/catalog-search.yaml
  - openapi/catalog.yaml
  - openapi/commerce-extensions.yaml
  - openapi/currencies.yaml
  - openapi/customer-addresses.yaml
  - openapi/exporter.yaml
  - openapi/files.yaml
  - openapi/flows.yaml
  - openapi/integrations.yaml
  - openapi/inventory-legacy.yaml
  - openapi/inventory.yaml
  - openapi/merchant-realm-mappings.yaml
  - openapi/permissions.yaml
  - openapi/personal-data.yaml
  - openapi/pim.yaml
  - openapi/pricebooks.yaml
  - openapi/promotions-builder.yaml
  - openapi/promotions.yaml
  - openapi/settings.yaml
  - openapi/single-sign-on.yaml
  - openapi/subscriptions.yaml
  type: http
slug: elastic-path-authentication
source_filename: elastic-path-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/account-addresses.yaml, openapi/accounts.yaml, openapi/application-keys.yaml,\n  openapi/carts.yaml, openapi/catalog-search.yaml, openapi/catalog.yaml, openapi/commerce-extensions.yaml,\n  openapi/currencies.yaml, openapi/customer-addresses.yaml, openapi/exporter.yaml, openapi/files.yaml,\n  openapi/flows.yaml ...\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerToken\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/account-addresses.yaml\n  - openapi/accounts.yaml\n  - openapi/application-keys.yaml\n  - openapi/carts.yaml\n  - openapi/catalog-search.yaml\n  - openapi/catalog.yaml\n  - openapi/commerce-extensions.yaml\n  - openapi/currencies.yaml\n  - openapi/customer-addresses.yaml\n  - openapi/exporter.yaml\n  - openapi/files.yaml\n  - openapi/flows.yaml\n  - openapi/integrations.yaml\n  - openapi/inventory-legacy.yaml\n  - openapi/inventory.yaml\n  - openapi/merchant-realm-mappings.yaml\n  - openapi/permissions.yaml\n\
  \  - openapi/personal-data.yaml\n  - openapi/pim.yaml\n  - openapi/pricebooks.yaml\n  - openapi/promotions-builder.yaml\n  - openapi/promotions.yaml\n  - openapi/settings.yaml\n  - openapi/single-sign-on.yaml\n  - openapi/subscriptions.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elastic-path/refs/heads/main/authentication/elastic-path-authentication.yml
summary_line: http · 1 scheme
tags:
- Commerce
- Headless Commerce
- Composable Commerce
- eCommerce
- B2B
- Products
- Catalogs
- Orders
- Promotions
- Subscriptions
- Payments
---

---
anonymous_access: false
api_key_in: []
api_specs:
- filename: canto-bulk-products-catalogs-api-openapi.yml
  format: yaml
  label: Canto Bulk Products Catalogs API
  slug: canto-bulk-products-catalogs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canto/refs/heads/main/openapi/canto-bulk-products-catalogs-api-openapi.yml
- filename: canto-bulk-products-channel-templates-api-openapi.yml
  format: yaml
  label: Canto Bulk Products Channel Templates API
  slug: canto-bulk-products-channel-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canto/refs/heads/main/openapi/canto-bulk-products-channel-templates-api-openapi.yml
- filename: canto-dimensions-api-openapi.yml
  format: yaml
  label: Canto Dimensions API
  slug: canto-dimensions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canto/refs/heads/main/openapi/canto-dimensions-api-openapi.yml
- filename: canto-filter-api-openapi.yml
  format: yaml
  label: Canto Filter API
  slug: canto-filter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canto/refs/heads/main/openapi/canto-filter-api-openapi.yml
- filename: canto-import-settings-api-openapi.yml
  format: yaml
  label: Canto Import Settings API
  slug: canto-import-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canto/refs/heads/main/openapi/canto-import-settings-api-openapi.yml
- filename: canto-imports-api-openapi.yml
  format: yaml
  label: Canto Imports API
  slug: canto-imports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canto/refs/heads/main/openapi/canto-imports-api-openapi.yml
- filename: canto-options-api-openapi.yml
  format: yaml
  label: Canto Options API
  slug: canto-options-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canto/refs/heads/main/openapi/canto-options-api-openapi.yml
- filename: canto-product-catalog-products-api-openapi.yml
  format: yaml
  label: Canto Product Catalog Products API
  slug: canto-product-catalog-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canto/refs/heads/main/openapi/canto-product-catalog-products-api-openapi.yml
- filename: canto-product-catalogs-api-openapi.yml
  format: yaml
  label: Canto Product Catalogs API
  slug: canto-product-catalogs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canto/refs/heads/main/openapi/canto-product-catalogs-api-openapi.yml
- filename: canto-product-categories-api-openapi.yml
  format: yaml
  label: Canto Product Categories API
  slug: canto-product-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canto/refs/heads/main/openapi/canto-product-categories-api-openapi.yml
- filename: canto-product-channel-template-products-api-openapi.yml
  format: yaml
  label: Canto Product Channel Template Products API
  slug: canto-product-channel-template-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canto/refs/heads/main/openapi/canto-product-channel-template-products-api-openapi.yml
- filename: canto-product-channel-templates-api-openapi.yml
  format: yaml
  label: Canto Product Channel Templates API
  slug: canto-product-channel-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canto/refs/heads/main/openapi/canto-product-channel-templates-api-openapi.yml
- filename: canto-product-custom-attributes-api-openapi.yml
  format: yaml
  label: Canto Product Custom Attributes API
  slug: canto-product-custom-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canto/refs/heads/main/openapi/canto-product-custom-attributes-api-openapi.yml
- filename: canto-product-share-links-api-openapi.yml
  format: yaml
  label: Canto Product Share Links API
  slug: canto-product-share-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canto/refs/heads/main/openapi/canto-product-share-links-api-openapi.yml
- filename: canto-product-types-api-openapi.yml
  format: yaml
  label: Canto Product Types API
  slug: canto-product-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canto/refs/heads/main/openapi/canto-product-types-api-openapi.yml
- filename: canto-products-api-openapi.yml
  format: yaml
  label: Canto Products API
  slug: canto-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canto/refs/heads/main/openapi/canto-products-api-openapi.yml
- filename: canto-variants-api-openapi.yml
  format: yaml
  label: Canto Variants API
  slug: canto-variants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canto/refs/heads/main/openapi/canto-variants-api-openapi.yml
- filename: canto-webhook-events-api-openapi.yml
  format: yaml
  label: Canto Webhook Events API
  slug: canto-webhook-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canto/refs/heads/main/openapi/canto-webhook-events-api-openapi.yml
- filename: canto-webhooks-api-openapi.yml
  format: yaml
  label: Canto Webhooks API
  slug: canto-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canto/refs/heads/main/openapi/canto-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Canto Authentication
name_suffix: Authentication
oauth_flows: []
overview: Canto secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Canto
provider_slug: canto
scheme_count: 1
schemes:
- bearerFormat: AccessToken
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/canto-pim-openapi.json
  type: http
slug: canto-authentication
source_filename: canto-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/canto-pim-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: AccessToken\n  sources:\n  - openapi/canto-pim-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/canto/refs/heads/main/authentication/canto-authentication.yml
summary_line: http · 1 scheme
tags:
- Digital Asset Management
- Brand Assets
- Image
- Video
- Documents
- Media Library
- Asset Distribution
---

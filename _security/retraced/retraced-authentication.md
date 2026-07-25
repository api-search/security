---
api_key_in:
- header
api_specs:
- filename: retraced-certificates-api-openapi.yml
  format: yaml
  label: Retraced Certificates API
  slug: retraced-certificates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retraced/refs/heads/main/openapi/retraced-certificates-api-openapi.yml
- filename: retraced-companies-api-openapi.yml
  format: yaml
  label: Retraced Companies API
  slug: retraced-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retraced/refs/heads/main/openapi/retraced-companies-api-openapi.yml
- filename: retraced-files-api-openapi.yml
  format: yaml
  label: Retraced Files API
  slug: retraced-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retraced/refs/heads/main/openapi/retraced-files-api-openapi.yml
- filename: retraced-guides-api-openapi.yml
  format: yaml
  label: Retraced Guides API
  slug: retraced-guides-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retraced/refs/heads/main/openapi/retraced-guides-api-openapi.yml
- filename: retraced-order-hub-attachment-templates-api-openapi.yml
  format: yaml
  label: Retraced Order Hub / Attachment Templates API
  slug: retraced-order-hub-attachment-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retraced/refs/heads/main/openapi/retraced-order-hub-attachment-templates-api-openapi.yml
- filename: retraced-order-hub-order-lines-api-openapi.yml
  format: yaml
  label: Retraced Order Hub / Order Lines API
  slug: retraced-order-hub-order-lines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retraced/refs/heads/main/openapi/retraced-order-hub-order-lines-api-openapi.yml
- filename: retraced-order-hub-orders-api-openapi.yml
  format: yaml
  label: Retraced Order Hub / Orders API
  slug: retraced-order-hub-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retraced/refs/heads/main/openapi/retraced-order-hub-orders-api-openapi.yml
- filename: retraced-product-bom-headers-api-openapi.yml
  format: yaml
  label: Retraced Product / BOM Headers API
  slug: retraced-product-bom-headers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retraced/refs/heads/main/openapi/retraced-product-bom-headers-api-openapi.yml
- filename: retraced-product-bom-lines-api-openapi.yml
  format: yaml
  label: Retraced Product / BOM Lines API
  slug: retraced-product-bom-lines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retraced/refs/heads/main/openapi/retraced-product-bom-lines-api-openapi.yml
- filename: retraced-product-bom-placements-api-openapi.yml
  format: yaml
  label: Retraced Product / BOM Placements API
  slug: retraced-product-bom-placements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retraced/refs/heads/main/openapi/retraced-product-bom-placements-api-openapi.yml
- filename: retraced-product-material-headers-api-openapi.yml
  format: yaml
  label: Retraced Product / Material Headers API
  slug: retraced-product-material-headers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retraced/refs/heads/main/openapi/retraced-product-material-headers-api-openapi.yml
- filename: retraced-product-material-lines-api-openapi.yml
  format: yaml
  label: Retraced Product / Material Lines API
  slug: retraced-product-material-lines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retraced/refs/heads/main/openapi/retraced-product-material-lines-api-openapi.yml
- filename: retraced-product-style-properties-api-openapi.yml
  format: yaml
  label: Retraced Product / Style Properties API
  slug: retraced-product-style-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retraced/refs/heads/main/openapi/retraced-product-style-properties-api-openapi.yml
- filename: retraced-product-style-types-api-openapi.yml
  format: yaml
  label: Retraced Product / Style Types API
  slug: retraced-product-style-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retraced/refs/heads/main/openapi/retraced-product-style-types-api-openapi.yml
- filename: retraced-product-styles-api-openapi.yml
  format: yaml
  label: Retraced Product / Styles API
  slug: retraced-product-styles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retraced/refs/heads/main/openapi/retraced-product-styles-api-openapi.yml
- filename: retraced-product-supply-chains-api-openapi.yml
  format: yaml
  label: Retraced Product / Supply Chains API
  slug: retraced-product-supply-chains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retraced/refs/heads/main/openapi/retraced-product-supply-chains-api-openapi.yml
- filename: retraced-release-notes-api-openapi.yml
  format: yaml
  label: Retraced Release Notes API
  slug: retraced-release-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retraced/refs/heads/main/openapi/retraced-release-notes-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Retraced Authentication
name_suffix: Authentication
oauth_flows: []
overview: Retraced secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Retraced
provider_slug: retraced
scheme_count: 1
schemes:
- description: Set the request header `companyapikey` to the value of an API key created in the Retraced Platform under Developers HQ > API Keys. Keys are shown once at creation. A single key is scoped to both the staging and production environments. If Developers HQ is not visible in the sidebar, a Customer Success Manager must enable it for the account.
  in: header
  name: companyApiKey
  parameter: companyapikey
  sources:
  - openapi/retraced-openapi-original.json
  type: apiKey
slug: retraced-authentication
source_filename: retraced-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://publicapi.retraced.com/\ndocs: https://publicapi.retraced.com/\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nnote: >-\n  The Retraced Public API OpenAPI does not declare securitySchemes; the auth model\n  below is captured verbatim from the published API reference. Authentication is\n  passwordless via a company-scoped API key sent in an HTTP header.\nschemes:\n  - name: companyApiKey\n    type: apiKey\n    in: header\n    parameter: companyapikey\n    description: >-\n      Set the request header `companyapikey` to the value of an API key created in the\n      Retraced Platform under Developers HQ > API Keys. Keys are shown once at creation.\n      A single key is scoped to both the staging and production environments. If\n      Developers HQ is not visible in the sidebar, a Customer Success Manager must\n      enable it for the account.\n    sources: [openapi/retraced-openapi-original.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/retraced/refs/heads/main/authentication/retraced-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Applicative Saas
- Supply Chain
- Sustainability
- Compliance
- Fashion
- Traceability
- Digital Product Passport
- ESG
---

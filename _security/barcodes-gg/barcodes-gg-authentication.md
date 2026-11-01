---
anonymous_access: false
api_key_in: []
api_specs:
- filename: barcodes-gg-account-api-openapi.yml
  format: yaml
  label: Barcodes.GG Account API
  slug: barcodes-gg-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/barcodes-gg/openapi/barcodes-gg-account-api-openapi.yml
- filename: barcodes-gg-barcodes-api-openapi.yml
  format: yaml
  label: Barcodes.GG Barcodes API
  slug: barcodes-gg-barcodes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/barcodes-gg/openapi/barcodes-gg-barcodes-api-openapi.yml
- filename: barcodes-gg-images-api-openapi.yml
  format: yaml
  label: Barcodes.GG Images API
  slug: barcodes-gg-images-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/barcodes-gg/openapi/barcodes-gg-images-api-openapi.yml
- filename: barcodes-gg-legacy-v1-api-openapi.yml
  format: yaml
  label: Barcodes.GG Legacy v1 API
  slug: barcodes-gg-legacy-v1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/barcodes-gg/openapi/barcodes-gg-legacy-v1-api-openapi.yml
- filename: barcodes-gg-products-api-openapi.yml
  format: yaml
  label: Barcodes.GG Products API
  slug: barcodes-gg-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/barcodes-gg/openapi/barcodes-gg-products-api-openapi.yml
auth_types: []
description: Authentication schemes as published on Barcodes.GG documentation.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Barcodes Gg Authentication
name_suffix: Authentication
oauth_flows: []
overview: Barcodes.GG declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Barcodes.GG
provider_slug: barcodes-gg
scheme_count: 1
schemes:
- evidence: Include your API token as a Bearer token in the Authorization header.
  header: Authorization
  how_to_obtain: Create one from the tokens section of your dashboard.
  location: header
  name: Bearer
  type: http-bearer
slug: barcodes-gg-authentication
source_filename: barcodes-gg-authentication.yml
source_heading: Authentication Profile
source_url: https://barcodes.gg/guide/docs/api-instructions/v2-overview/
source_yaml: "generated: '2026-10-21'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://barcodes.gg/guide/docs/api-instructions/v2-overview/\nsources:\n- https://barcodes.gg/guide/docs/api-instructions/v2-overview/\n- https://barcodes.gg/guide/docs/api-instructions/token-usage/\n- https://barcodes.gg/guide/docs/membership-plans/\n- https://barcodes.gg/blog/getting-started-barcodes-gg-api\ndescription: Authentication schemes as published on Barcodes.GG documentation.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: Include your API token as a Bearer token in the Authorization header.\n  location: header\n  header: Authorization\n  how_to_obtain: Create one from the tokens section of your dashboard.\ndocs: https://barcodes.gg/guide/docs/api-instructions/v2-overview/\n"
source_yaml_url: https://artifacts.apis.io/barcodes-gg/authentication/barcodes-gg-authentication.yml
summary_line: 1 scheme
tags:
- Company
- API
- Barcode
- Sneaker
- Streetwear
---

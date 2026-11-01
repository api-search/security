---
anonymous_access: false
api_key_in: []
api_specs:
- filename: catalogapi-com-cart-api-openapi.yml
  format: yaml
  label: catalogapi-com Cart API
  slug: catalogapi-com-cart-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/catalogapi-com/openapi/catalogapi-com-cart-api-openapi.yml
- filename: catalogapi-com-catalog-api-openapi.yml
  format: yaml
  label: catalogapi-com Catalog API
  slug: catalogapi-com-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/catalogapi-com/openapi/catalogapi-com-catalog-api-openapi.yml
- filename: catalogapi-com-health-api-openapi.yml
  format: yaml
  label: catalogapi-com Health API
  slug: catalogapi-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/catalogapi-com/openapi/catalogapi-com-health-api-openapi.yml
- filename: catalogapi-com-order-api-openapi.yml
  format: yaml
  label: catalogapi-com Order API
  slug: catalogapi-com-order-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/catalogapi-com/openapi/catalogapi-com-order-api-openapi.yml
auth_types: []
description: CatalogAPI uses API keys sent as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Catalogapi Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: catalogapi-com declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: catalogapi-com
provider_slug: catalogapi-com
scheme_count: 1
schemes:
- evidence: 'Send it as: `Authorization: Bearer YOUR_API_KEY`'
  header: Authorization
  how_to_obtain: Create a key from the dashboard after signing in.
  location: header
  name: Bearer
  type: http-bearer
slug: catalogapi-com-authentication
source_filename: catalogapi-com-authentication.yml
source_heading: Authentication Profile
source_url: https://catalogapi.com:443/auth.md
source_yaml: "generated: '2026-10-30'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://catalogapi.com:443/auth.md\nsources:\n- https://catalogapi.com:443/auth.md\n- https://catalogapi.com:443/.well-known/oauth-protected-resource\n- https://catalogapi.com/api/docs?view=auth\ndescription: CatalogAPI uses API keys sent as a Bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Send it as: `Authorization: Bearer YOUR_API_KEY`'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key from the dashboard after signing in.\nnote: No OAuth flows are supported.\ndocs: https://catalogapi.com:443/auth.md\n"
source_yaml_url: https://artifacts.apis.io/catalogapi-com/authentication/catalogapi-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- API
- Rewards
- GiftCards
- Global
---

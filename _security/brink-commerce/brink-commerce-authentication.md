---
anonymous_access: false
api_key_in: []
api_specs:
- filename: brink-commerce-openapi-generated.yml
  format: yaml
  label: Brink Commerce API
  slug: brink-commerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brink-commerce/refs/heads/main/openapi/_ae-authored/brink-commerce-openapi-generated.yml
auth_types: []
description: Authentication methods for Brink Commerce APIs
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Brink Commerce Authentication
name_suffix: Authentication
oauth_flows: []
overview: Brink Commerce declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Brink Commerce
provider_slug: brink-commerce
scheme_count: 2
schemes:
- evidence: '* `Authorization: Bearer {access_token}`

    * `x-api-key: {api_key}`'
  flows:
  - client_credentials
  header: Authorization
  how_to_obtain: Obtain `client_id`, `client_secret`, and `x-api-key` from the Merchant Portal
  location: header
  name: OAuth2
  scopes:
  - product-management/addon:read
  - product-management/product:write
  - product-management/addon:write
  - product-management/product:read
  token_url: /oauth2/token
  type: oauth2
- evidence: '* `x-api-key: {api_key}`'
  header: x-api-key
  how_to_obtain: Obtain `x-api-key` from the Merchant Portal
  location: header
  name: x-api-key
  type: apiKey
slug: brink-commerce-authentication
source_filename: brink-commerce-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.brinkcommerce.com/getting-started/essentials/authentication.md
source_yaml: "generated: '2026-10-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.brinkcommerce.com/getting-started/essentials/authentication.md\nsources:\n- https://docs.brinkcommerce.com/getting-started/essentials/authentication.md\n- https://docs.brinkcommerce.com/getting-started/essentials.md\n- https://docs.brinkcommerce.com/getting-started/essentials/api-architecture.md\n- https://docs.brinkcommerce.com/getting-started/guides.md\ndescription: Authentication methods for Brink Commerce APIs\nschemes:\n- type: oauth2\n  name: OAuth2\n  evidence: '* `Authorization: Bearer {access_token}`\n\n    * `x-api-key: {api_key}`'\n  location: header\n  header: Authorization\n  flows:\n  - client_credentials\n  token_url: /oauth2/token\n  scopes:\n  - product-management/addon:read\n  - product-management/product:write\n  - product-management/addon:write\n  - product-management/product:read\n  how_to_obtain: Obtain `client_id`, `client_secret`, and `x-api-key`\
  \ from the Merchant Portal\n- type: apiKey\n  name: x-api-key\n  evidence: '* `x-api-key: {api_key}`'\n  location: header\n  header: x-api-key\n  how_to_obtain: Obtain `x-api-key` from the Merchant Portal\ndocs: https://docs.brinkcommerce.com/getting-started/essentials/authentication.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brink-commerce/refs/heads/main/authentication/brink-commerce-authentication.yml
summary_line: 2 schemes
tags:
- eCommerce
- API
- Platform
- Enterprise
- Composable
---

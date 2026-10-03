---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bootic-catalog-api-openapi.yml
  format: yaml
  label: Bootic Catalog API
  slug: bootic-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bootic/refs/heads/main/openapi/bootic-catalog-api-openapi.yml
- filename: bootic-collections-api-openapi.yml
  format: yaml
  label: Bootic Collections API
  slug: bootic-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bootic/refs/heads/main/openapi/bootic-collections-api-openapi.yml
- filename: bootic-content-api-openapi.yml
  format: yaml
  label: Bootic Content API
  slug: bootic-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bootic/refs/heads/main/openapi/bootic-content-api-openapi.yml
- filename: bootic-customers-api-openapi.yml
  format: yaml
  label: Bootic Customers API
  slug: bootic-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bootic/refs/heads/main/openapi/bootic-customers-api-openapi.yml
- filename: bootic-orders-api-openapi.yml
  format: yaml
  label: Bootic Orders API
  slug: bootic-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bootic/refs/heads/main/openapi/bootic-orders-api-openapi.yml
- filename: bootic-price-lists-api-openapi.yml
  format: yaml
  label: Bootic Price Lists API
  slug: bootic-price-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bootic/refs/heads/main/openapi/bootic-price-lists-api-openapi.yml
- filename: bootic-product-types-api-openapi.yml
  format: yaml
  label: Bootic Product Types API
  slug: bootic-product-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bootic/refs/heads/main/openapi/bootic-product-types-api-openapi.yml
- filename: bootic-products-api-openapi.yml
  format: yaml
  label: Bootic Products API
  slug: bootic-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bootic/refs/heads/main/openapi/bootic-products-api-openapi.yml
- filename: bootic-promotions-api-openapi.yml
  format: yaml
  label: Bootic Promotions API
  slug: bootic-promotions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bootic/refs/heads/main/openapi/bootic-promotions-api-openapi.yml
- filename: bootic-root-api-openapi.yml
  format: yaml
  label: Bootic Root API
  slug: bootic-root-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bootic/refs/heads/main/openapi/bootic-root-api-openapi.yml
- filename: bootic-sellers-api-openapi.yml
  format: yaml
  label: Bootic Sellers API
  slug: bootic-sellers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bootic/refs/heads/main/openapi/bootic-sellers-api-openapi.yml
- filename: bootic-shops-api-openapi.yml
  format: yaml
  label: Bootic Shops API
  slug: bootic-shops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bootic/refs/heads/main/openapi/bootic-shops-api-openapi.yml
- filename: bootic-store-api-openapi.yml
  format: yaml
  label: Bootic Store API
  slug: bootic-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bootic/refs/heads/main/openapi/bootic-store-api-openapi.yml
- filename: bootic-subscriptions-api-openapi.yml
  format: yaml
  label: Bootic Subscriptions API
  slug: bootic-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bootic/refs/heads/main/openapi/bootic-subscriptions-api-openapi.yml
- filename: bootic-themes-api-openapi.yml
  format: yaml
  label: Bootic Themes API
  slug: bootic-themes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bootic/refs/heads/main/openapi/bootic-themes-api-openapi.yml
- filename: bootic-variants-api-openapi.yml
  format: yaml
  label: Bootic Variants API
  slug: bootic-variants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bootic/refs/heads/main/openapi/bootic-variants-api-openapi.yml
- filename: bootic-volume-discounts-api-openapi.yml
  format: yaml
  label: Bootic Volume Discounts API
  slug: bootic-volume-discounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bootic/refs/heads/main/openapi/bootic-volume-discounts-api-openapi.yml
- filename: bootic-wallets-api-openapi.yml
  format: yaml
  label: Bootic Wallets API
  slug: bootic-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bootic/refs/heads/main/openapi/bootic-wallets-api-openapi.yml
- filename: bootic-webhooks-api-openapi.yml
  format: yaml
  label: Bootic Webhooks API
  slug: bootic-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bootic/refs/heads/main/openapi/bootic-webhooks-api-openapi.yml
auth_types: []
description: Authentication methods for the Bolder API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Bootic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bootic declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Bootic
provider_slug: bootic
scheme_count: 2
schemes:
- evidence: 'curl -H "Authorization: Bearer $BOLDER_TOKEN " https://api.onbolder.com/v2'
  header: Authorization
  how_to_obtain: Create a token under Personal Access Tokens at https://auth.onbolder.com/dev/credentials and copy the shown token.
  location: header
  name: Personal Access Token
  type: http-bearer
- authorize_url: https://auth.onbolder.com/oauth/authorize
  evidence: The Bolder API uses OAuth 2.0 . The token must be sent in the Authorization header — query-parameter tokens are not accepted by v2.
  header: Authorization
  how_to_obtain: Register an application at https://auth.onbolder.com to obtain a CLIENT_ID and CLIENT_SECRET, then use one of the supported OAuth 2.0 grant types to obtain an access token.
  location: header
  name: OAuth 2.0
  token_url: https://auth.onbolder.com/oauth/token
  type: oauth2
slug: bootic-authentication
source_filename: bootic-authentication.yml
source_heading: Authentication Profile
source_url: https://api.onbolder.com/docs/v2#building-a-real-integration--register-an-oauth-application
source_yaml: "generated: '2026-10-02'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://api.onbolder.com/docs/v2#building-a-real-integration--register-an-oauth-application\nsources:\n- https://api.onbolder.com/docs/v2#building-a-real-integration--register-an-oauth-application\n- https://api.onbolder.com/docs/v2#authentication\n- https://api.onbolder.com/docs/v2#fastest-path--personal-access-token\n- https://api.onbolder.com/docs/v2#3-client-credentials-for-server-to-server--automated-scripts\ndescription: Authentication methods for the Bolder API\nschemes:\n- type: http-bearer\n  name: Personal Access Token\n  evidence: 'curl -H \"Authorization: Bearer $BOLDER_TOKEN \" https://api.onbolder.com/v2'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a token under Personal Access Tokens at https://auth.onbolder.com/dev/credentials and copy the shown token.\n- type: oauth2\n  name: OAuth 2.0\n  evidence: The Bolder API uses OAuth 2.0 . The token\
  \ must be sent in the Authorization header — query-parameter tokens are not accepted by v2.\n  location: header\n  header: Authorization\n  token_url: https://auth.onbolder.com/oauth/token\n  authorize_url: https://auth.onbolder.com/oauth/authorize\n  how_to_obtain: Register an application at https://auth.onbolder.com to obtain a CLIENT_ID and CLIENT_SECRET, then use one of the supported OAuth\n    2.0 grant types to obtain an access token.\nnote: 'OAuth 2.0 supports the following grant types: authorization_code, implicit, client_credentials, password, refresh_token (JWT Bearer).'\ndocs: https://api.onbolder.com/docs/v2#building-a-real-integration--register-an-oauth-application\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bootic/refs/heads/main/authentication/bootic-authentication.yml
summary_line: 2 schemes
tags:
- e-commerce
- marketplace
- Chile
- platform
- retail
---

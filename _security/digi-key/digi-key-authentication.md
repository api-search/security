---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: digi-key-barcoding-api-openapi.yml
  format: yaml
  label: Digi-Key Barcoding API
  slug: digi-key-barcoding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digi-key/refs/heads/main/openapi/digi-key-barcoding-api-openapi.yml
- filename: digi-key-bondedinventory-api-openapi.yml
  format: yaml
  label: Digi-Key Bonded Inventory API
  slug: digi-key-bondedinventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digi-key/refs/heads/main/openapi/digi-key-bondedinventory-api-openapi.yml
- filename: digi-key-customerresource-api-openapi.yml
  format: yaml
  label: Digi-Key Customer Resource API
  slug: digi-key-customerresource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digi-key/refs/heads/main/openapi/digi-key-customerresource-api-openapi.yml
- filename: digi-key-lists-api-openapi.yml
  format: yaml
  label: Digi-Key Lists API
  slug: digi-key-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digi-key/refs/heads/main/openapi/digi-key-lists-api-openapi.yml
- filename: digi-key-orderhistory-api-openapi.yml
  format: yaml
  label: Digi-Key Order History API
  slug: digi-key-orderhistory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digi-key/refs/heads/main/openapi/digi-key-orderhistory-api-openapi.yml
- filename: digi-key-ordermanagement-api-openapi.yml
  format: yaml
  label: Digi-Key Order Management API
  slug: digi-key-ordermanagement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digi-key/refs/heads/main/openapi/digi-key-ordermanagement-api-openapi.yml
- filename: digi-key-orders-api-openapi.yml
  format: yaml
  label: Digi-Key Orders API
  slug: digi-key-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digi-key/refs/heads/main/openapi/digi-key-orders-api-openapi.yml
- filename: digi-key-packlist-api-openapi.yml
  format: yaml
  label: Digi-Key Pack List API
  slug: digi-key-packlist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digi-key/refs/heads/main/openapi/digi-key-packlist-api-openapi.yml
- filename: digi-key-parts-api-openapi.yml
  format: yaml
  label: Digi-Key Parts API
  slug: digi-key-parts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digi-key/refs/heads/main/openapi/digi-key-parts-api-openapi.yml
- filename: digi-key-pcn-api-openapi.yml
  format: yaml
  label: Digi-Key Pcn API
  slug: digi-key-pcn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digi-key/refs/heads/main/openapi/digi-key-pcn-api-openapi.yml
- filename: digi-key-quotes-api-openapi.yml
  format: yaml
  label: Digi-Key Quotes API
  slug: digi-key-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digi-key/refs/heads/main/openapi/digi-key-quotes-api-openapi.yml
- filename: digi-key-product-search-api-openapi.yml
  format: yaml
  label: Digi-Key Product Search API
  slug: digi-key-product-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digi-key/refs/heads/main/openapi/digi-key-product-search-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: derived
name: Digi Key Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Digi-Key secures its APIs with apiKey and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Digi-Key
provider_slug: digi-key
scheme_count: 3
schemes:
- in: header
  name: apiKeySecurity
  parameter: X-DIGIKEY-Client-Id
  sources:
  - openapi/digi-key-b2bapi-order-management-api-ordermanagement-v1-openapi.yml
  - openapi/digi-key-barcoding-barcoding-v3-openapi.yml
  - openapi/digi-key-customerresource-customerresource-v1-openapi.yml
  - openapi/digi-key-mylists-api-mylists-v1-openapi.yml
  - openapi/digi-key-ordering-api-v3-ordering-v3-openapi.yml
  - openapi/digi-key-orderstatus-orderstatus-v4-openapi.yml
  - openapi/digi-key-packinglist-api-packinglist-openapi.yml
  - openapi/digi-key-product-change-notifications-api-changenotifications-v3-openapi.yml
  - openapi/digi-key-productsearch-api-products-v4-openapi.yml
  - openapi/digi-key-quote-api-quoting-v4-openapi.yml
  - openapi/digi-key-supply-chain-api-supplychain-v1-openapi.yml
  type: apiKey
- flows:
  - authorizationUrl: https://api.digikey.com/v1/oauth2/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://api.digikey.com/v1/oauth2/token
  name: oauth2AccessCodeSecurity
  sources:
  - openapi/digi-key-b2bapi-order-management-api-ordermanagement-v1-openapi.yml
  - openapi/digi-key-barcoding-barcoding-v3-openapi.yml
  - openapi/digi-key-ordering-api-v3-ordering-v3-openapi.yml
  - openapi/digi-key-packinglist-api-packinglist-openapi.yml
  - openapi/digi-key-product-change-notifications-api-changenotifications-v3-openapi.yml
  - openapi/digi-key-quote-api-quoting-v4-openapi.yml
  type: oauth2
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.digikey.com/v1/oauth2/token
  name: oauth2ApplicationSecurity
  sources:
  - openapi/digi-key-customerresource-customerresource-v1-openapi.yml
  - openapi/digi-key-mylists-api-mylists-v1-openapi.yml
  - openapi/digi-key-orderstatus-orderstatus-v4-openapi.yml
  - openapi/digi-key-productsearch-api-products-v4-openapi.yml
  - openapi/digi-key-supply-chain-api-supplychain-v1-openapi.yml
  type: oauth2
slug: digi-key-authentication
source_filename: digi-key-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: derived\nsource: openapi/digi-key-b2bapi-order-management-api-ordermanagement-v1-openapi.yml, openapi/digi-key-barcoding-barcoding-v3-openapi.yml,\n  openapi/digi-key-customerresource-customerresource-v1-openapi.yml, openapi/digi-key-mylists-api-mylists-v1-openapi.yml,\n  openapi/digi-key-ordering-api-v3-ordering-v3-openapi.yml, openapi/digi-key-orderstatus-orderstatus-v4-openapi.yml,\n  openapi/digi-key-packinglist-api-packinglist-openapi.yml, openapi/digi-key-product-change-notifications-api-changenotifications-v3-openapi.yml,\n  openapi/digi-key-productsearch-api-products-v4-openapi.yml, openapi/digi-key-quote-api-quoting-v4-openapi.yml,\n  openapi/digi-key-supply-chain-api-supplychain-v1-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: apiKeySecurity\n  type: apiKey\n  in: header\n  parameter: X-DIGIKEY-Client-Id\n  sources:\n\
  \  - openapi/digi-key-b2bapi-order-management-api-ordermanagement-v1-openapi.yml\n  - openapi/digi-key-barcoding-barcoding-v3-openapi.yml\n  - openapi/digi-key-customerresource-customerresource-v1-openapi.yml\n  - openapi/digi-key-mylists-api-mylists-v1-openapi.yml\n  - openapi/digi-key-ordering-api-v3-ordering-v3-openapi.yml\n  - openapi/digi-key-orderstatus-orderstatus-v4-openapi.yml\n  - openapi/digi-key-packinglist-api-packinglist-openapi.yml\n  - openapi/digi-key-product-change-notifications-api-changenotifications-v3-openapi.yml\n  - openapi/digi-key-productsearch-api-products-v4-openapi.yml\n  - openapi/digi-key-quote-api-quoting-v4-openapi.yml\n  - openapi/digi-key-supply-chain-api-supplychain-v1-openapi.yml\n- name: oauth2AccessCodeSecurity\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.digikey.com/v1/oauth2/authorize\n    tokenUrl: https://api.digikey.com/v1/oauth2/token\n    scopes: 0\n  sources:\n  - openapi/digi-key-b2bapi-order-management-api-ordermanagement-v1-openapi.yml\n\
  \  - openapi/digi-key-barcoding-barcoding-v3-openapi.yml\n  - openapi/digi-key-ordering-api-v3-ordering-v3-openapi.yml\n  - openapi/digi-key-packinglist-api-packinglist-openapi.yml\n  - openapi/digi-key-product-change-notifications-api-changenotifications-v3-openapi.yml\n  - openapi/digi-key-quote-api-quoting-v4-openapi.yml\n- name: oauth2ApplicationSecurity\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.digikey.com/v1/oauth2/token\n    scopes: 0\n  sources:\n  - openapi/digi-key-customerresource-customerresource-v1-openapi.yml\n  - openapi/digi-key-mylists-api-mylists-v1-openapi.yml\n  - openapi/digi-key-orderstatus-orderstatus-v4-openapi.yml\n  - openapi/digi-key-productsearch-api-products-v4-openapi.yml\n  - openapi/digi-key-supply-chain-api-supplychain-v1-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/digi-key/refs/heads/main/authentication/digi-key-authentication.yml
summary_line: apiKey/oauth2 · 3 schemes
tags:
- Shopping
- Public APIs
- Electronic Components
- Distribution
- Ordering
- Product Search
- Pricing
- Inventory
- Supply Chain
---

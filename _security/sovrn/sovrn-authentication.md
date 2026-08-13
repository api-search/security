---
api_key_in:
- header
api_specs:
- filename: sovrn-commerce-link-check-openapi.yml
  format: yaml
  label: Sovrn Commerce Link Check API
  slug: sovrn-commerce-link-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sovrn/refs/heads/main/openapi/sovrn-commerce-link-check-openapi.yml
- filename: sovrn-commerce-bid-check-openapi.yml
  format: yaml
  label: Sovrn Commerce Bid Check API
  slug: sovrn-commerce-bid-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sovrn/refs/heads/main/openapi/sovrn-commerce-bid-check-openapi.yml
- filename: sovrn-commerce-campaigns-openapi.yml
  format: yaml
  label: Sovrn Commerce Campaigns API
  slug: sovrn-commerce-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sovrn/refs/heads/main/openapi/sovrn-commerce-campaigns-openapi.yml
- filename: sovrn-commerce-reports-openapi.yml
  format: yaml
  label: Sovrn Commerce Real-Time Reports API
  slug: sovrn-commerce-real-time-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sovrn/refs/heads/main/openapi/sovrn-commerce-reports-openapi.yml
- filename: sovrn-merchant-summaries-openapi.yml
  format: yaml
  label: Sovrn Commerce Merchant Group Summaries API
  slug: sovrn-commerce-merchant-group-summaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sovrn/refs/heads/main/openapi/sovrn-merchant-summaries-openapi.yml
- filename: sovrn-product-recommendations-openapi.yml
  format: yaml
  label: Sovrn Commerce Product Recommendation API
  slug: sovrn-commerce-product-recommendation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sovrn/refs/heads/main/openapi/sovrn-product-recommendations-openapi.yml
- filename: sovrn-price-comparisons-openapi.yml
  format: yaml
  label: Sovrn Commerce Price Comparisons (Product Affiliate) API
  slug: sovrn-commerce-price-comparisons-product-affiliate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sovrn/refs/heads/main/openapi/sovrn-price-comparisons-openapi.yml
- filename: sovrn-product-coupons-openapi.yml
  format: yaml
  label: Sovrn Commerce Product Promo Codes API
  slug: sovrn-commerce-product-promo-codes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sovrn/refs/heads/main/openapi/sovrn-product-coupons-openapi.yml
- filename: sovrn-advertising-reporting-openapi.yml
  format: yaml
  label: Sovrn Advertising Performance Reporting API
  slug: sovrn-advertising-performance-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sovrn/refs/heads/main/openapi/sovrn-advertising-reporting-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Sovrn Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sovrn secures its APIs with apiKey across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Sovrn
provider_slug: sovrn
scheme_count: 5
schemes:
- in: header
  name: apiAuth
  parameter: x-api-key
  sources:
  - openapi/sovrn-advertising-reporting-openapi.yml
  type: apiKey
- in: header
  name: sec0
  parameter: authorization
  sources:
  - openapi/sovrn-commerce-campaigns-openapi.yml
  type: apiKey
  x-default: secret <secret key>
- in: header
  name: bearerAuth
  note: Named bearerAuth in the spec but declared as apiKey; the value is the Commerce Secret Key with the "secret " prefix, not an RFC 6750 bearer token.
  parameter: authorization
  sources:
  - openapi/sovrn-commerce-reports-openapi.yml
  type: apiKey
- description: 'Authorization header using the Secret Key scheme. Format: "secret {secret key}"'
  in: header
  name: SecretKey
  parameter: Authorization
  sources:
  - openapi/sovrn-merchant-summaries-openapi.yml
  - openapi/sovrn-product-coupons-openapi.yml
  type: apiKey
- in: header
  name: ApiKeyAuth
  parameter: authorization
  sources:
  - openapi/sovrn-price-comparisons-openapi.yml
  type: apiKey
slug: sovrn-authentication
source_filename: sovrn-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://developer.sovrn.com/docs/authorization\ndocs:\n- https://developer.sovrn.com/docs/authorization\n- https://knowledge.sovrn.com/kb/how-do-i-create-a-sovrn-api-key-for-the-ad-exchange-api\nderived_from: openapi/*.yml\nnote: >-\n  Sovrn runs two separate API-key regimes, one per product line, and they are not\n  interchangeable. Commerce (the former VigLink surface) authenticates with a per-site\n  Secret Key in an Authorization header using the literal prefix \"secret \" — the same\n  credential the Commerce MCP server takes. Advertising / Ad Exchange reporting\n  authenticates with an account-level key in an x-api-key header. There is no OAuth,\n  no OpenID Connect and no bearer-token flow on any published Sovrn API.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  regimes: 2\nregimes:\n- name: Commerce Secret Key\n  products: [Commerce, Commerce MCP]\n  scheme: apiKey\n  in: header\n\
  \  parameter: Authorization\n  format: 'secret {SECRET_KEY}'\n  note: >-\n    The word \"secret\" plus a space must precede the key value. Keys are per site (campaign),\n    not per account — different sites in one account carry different secret keys.\n  key_management:\n    console: https://platform.sovrn.com/commerce/settings\n    steps:\n    - Log in to the Sovrn Platform\n    - Go to Commerce Settings\n    - Under actions click the Key icon to view the API keys for that site\n    - If no secret key exists, click \"generate secret key\"\n    rotation: >-\n      A \"regenerate\" link invalidates the previous secret key immediately; every call using\n      the old key stops working until updated.\n  applies_to:\n  - openapi/sovrn-commerce-campaigns-openapi.yml\n  - openapi/sovrn-commerce-reports-openapi.yml\n  - openapi/sovrn-merchant-summaries-openapi.yml\n  - openapi/sovrn-product-coupons-openapi.yml\n  - openapi/sovrn-price-comparisons-openapi.yml\n  - mcp/sovrn-mcp.yml\n  unauthenticated_error:\n\
  \    status: 401\n    reason: invalidCredentials\n    message: >-\n      Authorization secret is missing or invalid. This can be found at\n      https://publishers.viglink.com/account and can be sent as a parameter or\n      Authorization header\n- name: Advertising API Key\n  products: [Ad Exchange, Advertising performance reporting]\n  scheme: apiKey\n  in: header\n  parameter: x-api-key\n  format: '{7-character prefix}.{32-character UUID}'\n  note: >-\n    Only the account owner can create or delete keys; there is no limit on the number of\n    keys and every key grants full access to all Advertising reporting data for the account.\n    The key value is displayed once at creation and cannot be retrieved afterwards.\n  key_management:\n    console: https://platform.sovrn.com/account/api-keys\n    rotation: Delete the key and create a new one; there is no in-place rotation.\n  applies_to:\n  - openapi/sovrn-advertising-reporting-openapi.yml\n- name: Campaign API key (query parameter)\n\
  \  products: [Commerce link building]\n  scheme: apiKey\n  in: query\n  parameter: key\n  note: >-\n    Affiliate link construction (sovrn.co?key=…&u=…) and the Link Check API take the\n    campaign's public API key as a URL parameter rather than a header. This is a link-signing\n    key, not the Secret Key, and is exposed in the rendered page by design.\n  applies_to:\n  - openapi/sovrn-commerce-link-check-openapi.yml\n  - openapi/sovrn-commerce-bid-check-openapi.yml\nschemes:\n- name: apiAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/sovrn-advertising-reporting-openapi.yml\n- name: sec0\n  type: apiKey\n  in: header\n  parameter: authorization\n  x-default: 'secret <secret key>'\n  sources:\n  - openapi/sovrn-commerce-campaigns-openapi.yml\n- name: bearerAuth\n  type: apiKey\n  in: header\n  parameter: authorization\n  note: >-\n    Named bearerAuth in the spec but declared as apiKey; the value is the Commerce Secret Key\n    with the \"secret \"\
  \ prefix, not an RFC 6750 bearer token.\n  sources:\n  - openapi/sovrn-commerce-reports-openapi.yml\n- name: SecretKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Authorization header using the Secret Key scheme. Format: \"secret {secret key}\"'\n  sources:\n  - openapi/sovrn-merchant-summaries-openapi.yml\n  - openapi/sovrn-product-coupons-openapi.yml\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: authorization\n  sources:\n  - openapi/sovrn-price-comparisons-openapi.yml\ngaps:\n- >-\n  openapi/sovrn-commerce-link-check-openapi.yml and\n  openapi/sovrn-commerce-bid-check-openapi.yml declare no securitySchemes at all, even though\n  both require a campaign key as a query parameter.\n- >-\n  openapi/sovrn-product-recommendations-openapi.yml declares no securitySchemes, though the\n  docs describe an API-key rate-limit tier for it.\n- >-\n  Five different scheme names (sec0, bearerAuth, SecretKey, ApiKeyAuth, apiAuth) describe\n  what are really\
  \ only two credentials. The naming is inconsistent across Sovrn's specs.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sovrn/refs/heads/main/authentication/sovrn-authentication.yml
summary_line: apiKey · 5 schemes
tags:
- Company
- Adtech
- Advertising
- Monetization
- Affiliate Marketing
- Programmatic
- Publishers
- Commerce
- Data
- Reporting
- Product Data
- Agent Native
---

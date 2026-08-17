---
api_key_in:
- header
- query
api_specs:
- filename: viglink-account-api-openapi.yml
  format: yaml
  label: VigLink (Sovrn Commerce) Account API
  slug: viglink-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viglink/refs/heads/main/openapi/viglink-account-api-openapi.yml
- filename: viglink-ai-orchestration-api-openapi.yml
  format: yaml
  label: VigLink (Sovrn Commerce) Ai Orchestration API
  slug: viglink-ai-orchestration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viglink/refs/heads/main/openapi/viglink-ai-orchestration-api-openapi.yml
- filename: viglink-bid-api-openapi.yml
  format: yaml
  label: VigLink (Sovrn Commerce) Bid API
  slug: viglink-bid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viglink/refs/heads/main/openapi/viglink-bid-api-openapi.yml
- filename: viglink-link-api-openapi.yml
  format: yaml
  label: VigLink (Sovrn Commerce) Link API
  slug: viglink-link-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viglink/refs/heads/main/openapi/viglink-link-api-openapi.yml
- filename: viglink-merchant-group-summaries-api-openapi.yml
  format: yaml
  label: VigLink (Sovrn Commerce) Merchant Group Summaries API
  slug: viglink-merchant-group-summaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viglink/refs/heads/main/openapi/viglink-merchant-group-summaries-api-openapi.yml
- filename: viglink-product-coupons-api-openapi.yml
  format: yaml
  label: VigLink (Sovrn Commerce) Product Coupons API
  slug: viglink-product-coupons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viglink/refs/heads/main/openapi/viglink-product-coupons-api-openapi.yml
- filename: viglink-reports-api-openapi.yml
  format: yaml
  label: VigLink (Sovrn Commerce) reports API
  slug: viglink-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viglink/refs/heads/main/openapi/viglink-reports-api-openapi.yml
- filename: viglink-sites-api-openapi.yml
  format: yaml
  label: VigLink (Sovrn Commerce) Sites API
  slug: viglink-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viglink/refs/heads/main/openapi/viglink-sites-api-openapi.yml
auth_types:
- apiKey
description: 'Every Sovrn Commerce (formerly VigLink) API authenticates with a static, per-SITE API key. There is no OAuth, no OIDC, no mTLS, and no token exchange anywhere in the estate. Two key materials exist and they are not interchangeable: a SECRET key sent in the Authorization header for the authenticated data APIs and the MCP server, and a PUBLIC Commerce API key sent as a `key` query parameter on the link/bid check surface and embedded in the client-side JavaScript snippet.'
kind: authentication
layout: security
method: searched
name: Viglink Authentication
name_suffix: Authentication
oauth_flows: []
overview: VigLink (Sovrn Commerce) secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: VigLink (Sovrn Commerce)
provider_slug: viglink
scheme_count: 3
schemes:
- description: Site Secret Key. The literal word "secret", a single space, then the key. Sovrn's docs call out the space explicitly because omitting it is the common failure.
  format: secret {SECRET_KEY}
  in: header
  name: SecretKey
  parameter: Authorization
  provisioning:
    steps:
    - Log into the Sovrn Platform (https://platform.sovrn.com/)
    - Go to Commerce Settings
    - Under Actions, click the Key icon to view the API keys for that site
    - If no secret key exists, click "generate secret key"
    where: https://platform.sovrn.com/commerce/settings
  rotation:
    breaking: Sovrn warns that regenerating immediately breaks every call still using the old key — there is no overlap/grace window and no multi-key support, so rotation is a hard cutover.
    mechanism: A "regenerate" link on the same Commerce Settings screen invalidates the previous secret key and issues a new one.
    supported: true
  scope: per-site — "There will be different secret keys for different sites within the same account."
  sources:
  - openapi/viglink-merchant-group-summaries-api-openapi.yml
  - openapi/viglink-product-coupons-api-openapi.yml
  - https://developer.sovrn.com/docs/authorization
  - https://developer.sovrn.com/docs/mcp
  type: apiKey
  used_by:
  - Campaigns API
  - Real-Time Reports APIs
  - Merchant Group Summaries APIs
  - Product Promo Codes API
  - Price Comparisons API
  - Commerce MCP Server (https://mcp.sovrn.com/commerce)
- description: ReadMe-generated scheme name for the same Authorization header contract as SecretKey. The duplicate naming is an artifact of Sovrn's docs tooling, not two different credentials.
  in: header
  name: sec0
  parameter: authorization
  sources:
  - openapi/viglink-account-api-openapi.yml
  - openapi/viglink-sites-api-openapi.yml
  - openapi/viglink-reports-api-openapi.yml
  type: apiKey
- description: Public Commerce API key, found on the account page at commerce.sovrn.com and in Site Settings. Passed as a `key` query parameter.
  in: query
  name: CommerceApiKey
  parameter: key
  public: true
  public_note: This key is embedded in the client-side vglnk.js snippet and in wrapped affiliate link URLs (https://sovrn.co?key=YOUR_API_KEY&u=…), so it is public by design and must not be treated as a secret.
  sources:
  - https://developer.sovrn.com/reference/link
  - https://developer.sovrn.com/reference/building-affiliate-links
  type: apiKey
  used_by:
  - Link Check API
  - Bid Check API
  - Commerce JavaScript library (vglnk)
  - Affiliate link wrapping (sovrn.co)
slug: viglink-authentication
source_filename: viglink-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://developer.sovrn.com/docs/authorization\nderived_from:\n- openapi/viglink-account-api-openapi.yml\n- openapi/viglink-merchant-group-summaries-api-openapi.yml\n- openapi/viglink-sites-api-openapi.yml\n- openapi/viglink-product-coupons-api-openapi.yml\n- openapi/viglink-reports-api-openapi.yml\ndocs: https://developer.sovrn.com/docs/authorization\ndescription: >-\n  Every Sovrn Commerce (formerly VigLink) API authenticates with a static, per-SITE\n  API key. There is no OAuth, no OIDC, no mTLS, and no token exchange anywhere in the\n  estate. Two key materials exist and they are not interchangeable: a SECRET key sent\n  in the Authorization header for the authenticated data APIs and the MCP server, and\n  a PUBLIC Commerce API key sent as a `key` query parameter on the link/bid check\n  surface and embedded in the client-side JavaScript snippet.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\n  oauth2:\
  \ false\n  openid_connect: false\n  mutual_tls: false\n  scopes: false\n  scopes_note: >-\n    No OAuth scope surface exists, so no scopes/ artifact is emitted. Authorization is\n    all-or-nothing per site key.\nschemes:\n- name: SecretKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: secret {SECRET_KEY}\n  description: >-\n    Site Secret Key. The literal word \"secret\", a single space, then the key. Sovrn's\n    docs call out the space explicitly because omitting it is the common failure.\n  scope: per-site — \"There will be different secret keys for different sites within\n    the same account.\"\n  provisioning:\n    where: https://platform.sovrn.com/commerce/settings\n    steps:\n    - Log into the Sovrn Platform (https://platform.sovrn.com/)\n    - Go to Commerce Settings\n    - Under Actions, click the Key icon to view the API keys for that site\n    - If no secret key exists, click \"generate secret key\"\n  rotation:\n    supported: true\n    mechanism:\
  \ >-\n      A \"regenerate\" link on the same Commerce Settings screen invalidates the previous\n      secret key and issues a new one.\n    breaking: >-\n      Sovrn warns that regenerating immediately breaks every call still using the old\n      key — there is no overlap/grace window and no multi-key support, so rotation is\n      a hard cutover.\n  used_by:\n  - Campaigns API\n  - Real-Time Reports APIs\n  - Merchant Group Summaries APIs\n  - Product Promo Codes API\n  - Price Comparisons API\n  - Commerce MCP Server (https://mcp.sovrn.com/commerce)\n  sources:\n  - openapi/viglink-merchant-group-summaries-api-openapi.yml\n  - openapi/viglink-product-coupons-api-openapi.yml\n  - https://developer.sovrn.com/docs/authorization\n  - https://developer.sovrn.com/docs/mcp\n- name: sec0\n  type: apiKey\n  in: header\n  parameter: authorization\n  description: >-\n    ReadMe-generated scheme name for the same Authorization header contract as\n    SecretKey. The duplicate naming is an artifact\
  \ of Sovrn's docs tooling, not two\n    different credentials.\n  sources:\n  - openapi/viglink-account-api-openapi.yml\n  - openapi/viglink-sites-api-openapi.yml\n  - openapi/viglink-reports-api-openapi.yml\n- name: CommerceApiKey\n  type: apiKey\n  in: query\n  parameter: key\n  description: >-\n    Public Commerce API key, found on the account page at commerce.sovrn.com and in\n    Site Settings. Passed as a `key` query parameter.\n  public: true\n  public_note: >-\n    This key is embedded in the client-side vglnk.js snippet and in wrapped affiliate\n    link URLs (https://sovrn.co?key=YOUR_API_KEY&u=…), so it is public by design and\n    must not be treated as a secret.\n  used_by:\n  - Link Check API\n  - Bid Check API\n  - Commerce JavaScript library (vglnk)\n  - Affiliate link wrapping (sovrn.co)\n  sources:\n  - https://developer.sovrn.com/reference/link\n  - https://developer.sovrn.com/reference/building-affiliate-links\ntransport:\n  tls_minimum: TLS 1.2\n  tls_source: https://www.sovrn.com/about-sovrn/security/\n\
  observed:\n- url: https://viglink.io/v1/reports/transactions\n  unauthenticated_status: 401\n  checked: '2026-08-13'\n- url: https://viglink.io/merchants/rates/summaries/delta\n  unauthenticated_status: 401\n  checked: '2026-08-13'\n- url: https://mcp.sovrn.com/commerce\n  method: POST tools/list\n  unauthenticated_status: 401\n  body: '{\"error\":\"invalid_token\"}'\n  checked: '2026-08-13'\ngaps:\n- No OAuth 2.0 / OIDC option for delegated access — a third-party tool acting for a\n  publisher must hold that publisher's long-lived site Secret Key.\n- No scoped or read-only key variant; one key grants the full authenticated surface\n  for its site.\n- No key expiry, and rotation has no overlap window.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/viglink/refs/heads/main/authentication/viglink-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Affiliate Marketing
- Commerce
- Monetization
- Publishers
- Links
- Advertising
- Reporting
---

---
api_key_in:
- query
- path
api_specs:
- filename: zazzle-create-a-product-api-openapi.yml
  format: yaml
  label: Zazzle Create a Product API
  slug: zazzle-create-a-product-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zazzle/refs/heads/main/openapi/zazzle-create-a-product-api-openapi.yml
- filename: zazzle-realview-api-openapi.yml
  format: yaml
  label: Zazzle Real View API
  slug: zazzle-realview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zazzle/refs/heads/main/openapi/zazzle-realview-api-openapi.yml
- filename: zazzle-vendor-api-openapi.yml
  format: yaml
  label: Zazzle Vendor API
  slug: zazzle-vendor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zazzle/refs/heads/main/openapi/zazzle-vendor-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Zazzle Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zazzle secures its APIs with apiKey across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Zazzle
provider_slug: zazzle
scheme_count: 4
schemes:
- api: zazzle:create-a-product
  description: The partner's 18-digit Zazzle member account ID, carried in the path segment `at-<accountId>` (and as the `at` query parameter on the RealView service). It identifies the account the generated product is attributed to. It is not a secret — it appears in every public linkover URL.
  in: path
  name: memberAccountId
  parameter: at
  sources:
  - openapi/zazzle-create-a-product-openapi.yml
  - openapi/zazzle-realview-openapi.yml
  type: apiKey
- api: zazzle:create-a-product
  description: Optional 18-digit Zazzle Associate ID used for referral attribution and royalty crediting. Also not a secret.
  in: query
  name: associateId
  parameter: rf
  sources:
  - openapi/zazzle-create-a-product-openapi.yml
  type: apiKey
- api: zazzle:vendor
  description: Vendor identifier issued by Zazzle to an onboarded Maker.
  in: query
  name: vendorId
  parameter: vendorid
  sources:
  - openapi/zazzle-vendor-openapi.yml
  type: apiKey
- api: zazzle:vendor
  description: Per-call MD5 signature over the vendor id, the call's business parameters and the vendor's shared secret. Functions as a request signature rather than a static key — the shared secret itself is never transmitted.
  in: query
  name: callHash
  parameter: hash
  sources:
  - openapi/zazzle-vendor-openapi.yml
  type: apiKey
slug: zazzle-authentication
source_filename: zazzle-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nsource: openapi/zazzle-vendor-openapi.yml\ndocs: https://asset.zcache.com/assets/graphics/z4/uniquePages/zAPI/ZazzleApiGuide.v3.pdf\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\n  - path\n  oauth2_flows: []\n  note: >-\n    Zazzle publishes no OAuth 2.0, OIDC or bearer-token surface on any of its three public API\n    surfaces. Access is identifier-based (account/associate/vendor IDs carried in the URL) with a\n    per-call MD5 request signature on the partner-gated Vendor API only.\nschemes:\n- name: memberAccountId\n  type: apiKey\n  in: path\n  parameter: at\n  api: zazzle:create-a-product\n  description: >-\n    The partner's 18-digit Zazzle member account ID, carried in the path segment `at-<accountId>`\n    (and as the `at` query parameter on the RealView service). It identifies the account the\n    generated product is attributed to. It is not a secret — it appears in every public linkover URL.\n  sources:\n  -\
  \ openapi/zazzle-create-a-product-openapi.yml\n  - openapi/zazzle-realview-openapi.yml\n- name: associateId\n  type: apiKey\n  in: query\n  parameter: rf\n  api: zazzle:create-a-product\n  description: >-\n    Optional 18-digit Zazzle Associate ID used for referral attribution and royalty crediting. Also\n    not a secret.\n  sources:\n  - openapi/zazzle-create-a-product-openapi.yml\n- name: vendorId\n  type: apiKey\n  in: query\n  parameter: vendorid\n  api: zazzle:vendor\n  description: Vendor identifier issued by Zazzle to an onboarded Maker.\n  sources:\n  - openapi/zazzle-vendor-openapi.yml\n- name: callHash\n  type: apiKey\n  in: query\n  parameter: hash\n  api: zazzle:vendor\n  description: >-\n    Per-call MD5 signature over the vendor id, the call's business parameters and the vendor's shared\n    secret. Functions as a request signature rather than a static key — the shared secret itself is\n    never transmitted.\n  sources:\n  - openapi/zazzle-vendor-openapi.yml\nauthorization_model:\n\
  \  create_a_product:\n    style: origin-allowlist\n    description: >-\n      The Create-a-Product API has no credential in the conventional sense. Authorization is enforced\n      out of band by three account-level gates the partner must satisfy before linkovers render:\n      (1) enrollment in the Zazzle Associates Program, (2) acceptance of the Create-a-Product API\n      terms, and (3) declaration of the domains the partner's image URLs will be served from. An\n      image URL served from an undeclared domain fails with \"Zazzle API Error: Image failed to\n      upload\".\n    enrollment:\n    - https://www.zazzle.com/lgn/registration\n    - https://www.zazzle.com/my/associate/associate\n    - https://www.zazzle.com/my/associate/create_a_product_api_signup\n    - https://www.zazzle.com/my/associate/domains\n  vendor:\n    style: signed-request\n    description: >-\n      Zazzle-issued `vendorid` plus a per-call `hash`. Credentials are issued through Zazzle Maker\n      onboarding;\
  \ there is no public self-service signup and no documented rotation or revocation\n      endpoint.\n    contact: maker.management@zazzle.com\ngaps:\n- No OAuth 2.0 / OpenID Connect surface on any Zazzle API.\n- No bearer tokens, no scoped access, no per-integration key with revocation.\n- Vendor API credentials and the hash construction are documented only in the Maker-issued PDF.\n- Secrets travel in the query string on the Vendor API, so they land in access logs and referrers.\nx-evidence:\n- url: https://asset.zcache.com/assets/graphics/z4/uniquePages/zAPI/ZazzleApiGuide.v3.pdf\n  http_status: 200\n  content_type: application/pdf\n  fetched: '2026-08-05'\n- url: https://vendor.zazzle.com/v100/api.aspx?method=listneworders\n  http_status: 200\n  content_type: text/xml\n  fetched: '2026-08-05'\n  note: \"anonymous call returns Invalid parameter 'hash' — confirms hash is required\"\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zazzle/refs/heads/main/authentication/zazzle-authentication.yml
summary_line: apiKey · 4 schemes
tags:
- Company
- E-Commerce
- Marketplace
- Print On Demand
- Manufacturing
- Retail
- Affiliates
- Custom Products
- Order Management
- Shipping
---

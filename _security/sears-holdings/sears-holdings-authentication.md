---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Sears Holdings Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sears Holdings declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Sears Holdings
provider_slug: sears-holdings
scheme_count: 1
schemes:
- algorithm: HMAC-SHA256
  credential_scope: per seller account; secondary users must generate their own key
  documented: true
  header_format: HMAC-SHA256 emailaddress=<email address>,timestamp=<timestamp>,signature=<signature>
  id: hmac-sha256-authorization
  in: header
  label: HMAC-SHA256 request signing
  name: Authorization
  scheme: custom
  secret: base64-encoded seller secret key, self-generated in Seller Portal under Account Info
  signature_encoding: hexadecimal
  source: https://marketplace.sears.com/docs/api-guide/using-sear-marketplace-apis-for-xml-integration/credentials-and-authentication/
  string_to_sign: <sellerId>:<emailaddress>:<currentTimestamp>
  timestamp_format: yyyy-MM-dd'T'HH:mm:ss'Z' (UTC)
  timestamp_validity: 30 minutes
  type: http
slug: sears-holdings-authentication
source_filename: sears-holdings-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: searched\nsource: https://marketplace.sears.com/docs/api-guide/using-sear-marketplace-apis-for-xml-integration/credentials-and-authentication/\ndocs: https://marketplace.sears.com/seller-support/api-authentication-process/\napi: Sears Marketplace Seller API\nbase_url: https://seller.marketplace.sears.com/SellerPortal/api\nnote: >-\n  Derived by hand from the provider's own published API Guide rather than from an OpenAPI\n  securitySchemes block, because Sears Marketplace publishes no OpenAPI. The scheme is a custom\n  HMAC signature, not OAuth, not OpenID Connect and not a bearer token, so there is no scopes/\n  artifact for this provider.\nschemes:\n  - id: hmac-sha256-authorization\n    type: http\n    scheme: custom\n    in: header\n    name: Authorization\n    algorithm: HMAC-SHA256\n    label: HMAC-SHA256 request signing\n    header_format: \"HMAC-SHA256 emailaddress=<email address>,timestamp=<timestamp>,signature=<signature>\"\n    string_to_sign:\
  \ \"<sellerId>:<emailaddress>:<currentTimestamp>\"\n    timestamp_format: \"yyyy-MM-dd'T'HH:mm:ss'Z' (UTC)\"\n    timestamp_validity: 30 minutes\n    signature_encoding: hexadecimal\n    secret: base64-encoded seller secret key, self-generated in Seller Portal under Account Info\n    credential_scope: per seller account; secondary users must generate their own key\n    documented: true\n    source: https://marketplace.sears.com/docs/api-guide/using-sear-marketplace-apis-for-xml-integration/credentials-and-authentication/\noauth2: false\nopenid_connect: false\nmutual_tls: false\napi_keys: false\nscopes_published: false\ncredential_acquisition:\n  self_service: false\n  requires_account: true\n  steps:\n    - Apply to sell on Sears Marketplace at https://marketplace.sears.com/sell-on-sears/\n    - Log in to Seller Portal at https://seller.marketplace.sears.com\n    - Open your name menu (upper right) -> Account Info and generate the base64 secret key\n    - Compute the HMAC-SHA256 signature\
  \ per request and send it in the Authorization header\ndeprecated_schemes:\n  - id: email-password-in-url\n    retired: '2016-03-31'\n    note: >-\n      Before 2016-03-31 API URLs carried an email address and password. Those calls are now\n      rejected outright; the provider states this explicitly in the API Guide.\nunauthenticated_behavior:\n  probe: https://seller.marketplace.sears.com/SellerPortal/api/oms/purchaseorder/v19?sellerId=1234\n  observed: '2026-08-28'\n  http_status: 200\n  content_type: application/xml;charset=UTF-8\n  body: \"<api-response><error-detail>Missing Authorization header in request</error-detail></api-response>\"\n  note: >-\n    The API answers an unauthenticated call with HTTP 200 and an in-body error element rather than\n    401/403. Clients cannot rely on the status line to detect an auth failure.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sears-holdings/refs/heads/main/authentication/sears-holdings-authentication.yml
summary_line: 1 scheme
tags:
- Fortune 100
- Retail
- E-Commerce
- Marketplace
- Order Management
- Inventory
- Product Catalog
- Seller Integration
- XML
---

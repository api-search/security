---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Google Pay Authentication
name_suffix: Authentication
oauth_flows: []
overview: Google Pay declares 5 security scheme(s) across its OpenAPI definitions.
provider_name: Google Pay
provider_slug: google-pay
scheme_count: 5
schemes:
- applies_to:
  - Google Pay API (Web)
  - Google Pay API for Android
  credential_fields:
  - merchantId
  - merchantName
  description: 'The Google Pay Web and Android client APIs carry no bearer credential at all. Authorisation is an out-of-band merchant registration: a Google Pay Business Profile is created in the Google Pay & Wallet Console, the top-level domain calling the API is registered against it, the Google Pay API Terms of Service and Acceptable Use Policy are accepted, integration screenshots are submitted for Google review, and only after approval may the client pass environment PRODUCTION with a real merchantId in MerchantInfo.'
  docs: https://developers.google.com/pay/api/web/guides/test-and-deploy/deploy-production-environment
  environments:
  - TEST
  - PRODUCTION
  id: merchant-registration
  type: none
- applies_to:
  - Google Pay API (Web)
  - Google Pay API for Android
  description: Returned payment data is a signed and encrypted PaymentMethodToken. Google signs the token with its own keys and encrypts to the merchant's or gateway's public key using ECIES (Elliptic Curve Integrated Encryption Scheme). Protocol versions ECv1 and ECv2; ECv2 is the default for new integrations. Direct (non-gateway) integration requires the merchant to be PCI DSS compliant as validated by a Qualified Security Assessor.
  docs: https://developers.google.com/pay/api/web/guides/resources/payment-data-cryptography
  id: payment-token-cryptography
  key_material:
    test_signing_keys: https://payments.developers.google.com/paymentmethodtoken/test/keys.json
  type: message-signing
- applies_to:
  - Google Wallet API
  description: Google Wallet REST calls against walletobjects.googleapis.com are authorised with a Google Cloud service account key exchanged for an OAuth 2.0 access token. The single scope is the one declared in the Wallet API Discovery document.
  docs: https://developers.google.com/wallet/generic/rest/prerequisites
  evidence: discovery/google-pay-walletobjects-v1-discovery.json (auth.oauth2.scopes)
  flows:
  - jwt-bearer (Google service account)
  id: oauth2-service-account
  issuer: https://accounts.google.com
  scopes:
  - https://www.googleapis.com/auth/wallet_object.issuer
  token_endpoint: https://oauth2.googleapis.com/token
  type: oauth2
- api_keys_accepted: false
  applies_to:
  - Google Pay & Wallet Developer MCP server
  description: The MCP server at paydeveloper.googleapis.com authenticates with OAuth 2.0 client credentials plus Google Cloud IAM. Google states explicitly that the server does not accept API keys. tools/list is readable anonymously; tool invocation is not.
  docs: https://developers.google.com/pay/api/web/guides/use-pay-wallet-mcp
  flows:
  - authorization_code
  iam_role: roles/mcp.toolUser
  id: oauth2-mcp
  issuer: https://accounts.google.com
  scopes:
  - https://www.googleapis.com/auth/paydeveloper.merchant
  - https://www.googleapis.com/auth/paydeveloper.issuer.readonly
  type: oauth2
- algorithm: ES256
  applies_to:
  - Google Universal Commerce Protocol
  description: Google's UCP discovery profile at ucp.goog publishes four ES256 (P-256) JWK signing keys in both a signing_keys[] and a keys[] array, used to verify UCP payloads exchanged with Google's commerce surfaces.
  docs: https://developers.google.com/merchant/ucp/guides/ucp-profile
  evidence: well-known/google-pay-ucp-profile.json
  id: ucp-profile-signing
  type: message-signing
slug: google-pay-authentication
source_filename: google-pay-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "specification: API Commons Authentication\nspecificationVersion: '0.1'\nprovider: Google Pay\nproviderId: google-pay\ngenerated: '2026-09-12'\nmethod: searched\nsource: >-\n  https://developers.google.com/pay/api/web/guides/setup ·\n  https://developers.google.com/pay/api/web/guides/test-and-deploy/deploy-production-environment ·\n  https://developers.google.com/wallet/generic/rest/prerequisites ·\n  https://developers.google.com/pay/api/web/guides/use-pay-wallet-mcp ·\n  well-known/google-pay-accounts-openid-configuration.json (probed 2026-09-12)\nnote: >-\n  derive-authentication.py found no securitySchemes because Google publishes no OpenAPI for any\n  Google Pay surface. This profile was read from Google's own setup and prerequisite pages and\n  from the live OpenID discovery document at accounts.google.com. There is no single Google Pay\n  auth model — the surfaces authenticate four different ways, which is the finding.\nschemes:\n  - id: merchant-registration\n    applies_to:\n\
  \      - Google Pay API (Web)\n      - Google Pay API for Android\n    type: none\n    description: >-\n      The Google Pay Web and Android client APIs carry no bearer credential at all. Authorisation\n      is an out-of-band merchant registration: a Google Pay Business Profile is created in the\n      Google Pay & Wallet Console, the top-level domain calling the API is registered against it,\n      the Google Pay API Terms of Service and Acceptable Use Policy are accepted, integration\n      screenshots are submitted for Google review, and only after approval may the client pass\n      environment PRODUCTION with a real merchantId in MerchantInfo.\n    credential_fields:\n      - merchantId\n      - merchantName\n    environments:\n      - TEST\n      - PRODUCTION\n    docs: https://developers.google.com/pay/api/web/guides/test-and-deploy/deploy-production-environment\n  - id: payment-token-cryptography\n    applies_to:\n      - Google Pay API (Web)\n      - Google Pay API for Android\n\
  \    type: message-signing\n    description: >-\n      Returned payment data is a signed and encrypted PaymentMethodToken. Google signs the token\n      with its own keys and encrypts to the merchant's or gateway's public key using ECIES\n      (Elliptic Curve Integrated Encryption Scheme). Protocol versions ECv1 and ECv2; ECv2 is the\n      default for new integrations. Direct (non-gateway) integration requires the merchant to be\n      PCI DSS compliant as validated by a Qualified Security Assessor.\n    key_material:\n      test_signing_keys: https://payments.developers.google.com/paymentmethodtoken/test/keys.json\n    docs: https://developers.google.com/pay/api/web/guides/resources/payment-data-cryptography\n  - id: oauth2-service-account\n    applies_to:\n      - Google Wallet API\n    type: oauth2\n    flows:\n      - jwt-bearer (Google service account)\n    scopes:\n      - https://www.googleapis.com/auth/wallet_object.issuer\n    token_endpoint: https://oauth2.googleapis.com/token\n\
  \    issuer: https://accounts.google.com\n    description: >-\n      Google Wallet REST calls against walletobjects.googleapis.com are authorised with a Google\n      Cloud service account key exchanged for an OAuth 2.0 access token. The single scope is the\n      one declared in the Wallet API Discovery document.\n    evidence: discovery/google-pay-walletobjects-v1-discovery.json (auth.oauth2.scopes)\n    docs: https://developers.google.com/wallet/generic/rest/prerequisites\n  - id: oauth2-mcp\n    applies_to:\n      - Google Pay & Wallet Developer MCP server\n    type: oauth2\n    flows:\n      - authorization_code\n    scopes:\n      - https://www.googleapis.com/auth/paydeveloper.merchant\n      - https://www.googleapis.com/auth/paydeveloper.issuer.readonly\n    iam_role: roles/mcp.toolUser\n    api_keys_accepted: false\n    issuer: https://accounts.google.com\n    description: >-\n      The MCP server at paydeveloper.googleapis.com authenticates with OAuth 2.0 client\n      credentials\
  \ plus Google Cloud IAM. Google states explicitly that the server does not accept\n      API keys. tools/list is readable anonymously; tool invocation is not.\n    docs: https://developers.google.com/pay/api/web/guides/use-pay-wallet-mcp\n  - id: ucp-profile-signing\n    applies_to:\n      - Google Universal Commerce Protocol\n    type: message-signing\n    algorithm: ES256\n    description: >-\n      Google's UCP discovery profile at ucp.goog publishes four ES256 (P-256) JWK signing keys in\n      both a signing_keys[] and a keys[] array, used to verify UCP payloads exchanged with\n      Google's commerce surfaces.\n    evidence: well-known/google-pay-ucp-profile.json\n    docs: https://developers.google.com/merchant/ucp/guides/ucp-profile\nauthorization_server:\n  issuer: https://accounts.google.com\n  openid_configuration: https://accounts.google.com/.well-known/openid-configuration\n  oauth_authorization_server: https://accounts.google.com/.well-known/oauth-authorization-server\n \
  \ probed: '2026-09-12'\n  http_status: 200\n  files:\n    - well-known/google-pay-accounts-openid-configuration.json\n    - well-known/google-pay-accounts-oauth-authorization-server.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-pay/refs/heads/main/authentication/google-pay-authentication.yml
summary_line: 5 schemes
tags:
- Agentic Commerce
- Checkout
- Contactless Payments
- Digital Wallet
- Merchants
- Mobile Payments
- Payments
- Tokenization
---

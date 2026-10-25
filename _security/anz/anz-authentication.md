---
anonymous_access: true
api_key_in: []
api_specs:
- filename: anz-banking-account-balances-api-openapi.yml
  format: yaml
  label: Australia and New Zealand Banking Group (ANZ) Banking Account Balances API
  slug: anz-banking-account-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anz/refs/heads/main/openapi/anz-banking-account-balances-api-openapi.yml
- filename: anz-banking-account-direct-debits-api-openapi.yml
  format: yaml
  label: Australia and New Zealand Banking Group (ANZ) Banking Account Direct Debits API
  slug: anz-banking-account-direct-debits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anz/refs/heads/main/openapi/anz-banking-account-direct-debits-api-openapi.yml
- filename: anz-banking-account-scheduled-payments-api-openapi.yml
  format: yaml
  label: Australia and New Zealand Banking Group (ANZ) Banking Account Scheduled Payments API
  slug: anz-banking-account-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anz/refs/heads/main/openapi/anz-banking-account-scheduled-payments-api-openapi.yml
- filename: anz-banking-account-transactions-api-openapi.yml
  format: yaml
  label: Australia and New Zealand Banking Group (ANZ) Banking Account Transactions API
  slug: anz-banking-account-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anz/refs/heads/main/openapi/anz-banking-account-transactions-api-openapi.yml
- filename: anz-banking-accounts-api-openapi.yml
  format: yaml
  label: Australia and New Zealand Banking Group (ANZ) Banking Accounts API
  slug: anz-banking-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anz/refs/heads/main/openapi/anz-banking-accounts-api-openapi.yml
- filename: anz-banking-payees-api-openapi.yml
  format: yaml
  label: Australia and New Zealand Banking Group (ANZ) Banking Payees API
  slug: anz-banking-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anz/refs/heads/main/openapi/anz-banking-payees-api-openapi.yml
- filename: anz-banking-products-api-openapi.yml
  format: yaml
  label: Australia and New Zealand Banking Group (ANZ) Banking Products API
  slug: anz-banking-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anz/refs/heads/main/openapi/anz-banking-products-api-openapi.yml
- filename: anz-banking-products-api-openapi.yml
  format: yaml
  label: Australia and New Zealand Banking Group (ANZ) ANZ Plus Banking Products API
  slug: anz-plus-banking-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anz/refs/heads/main/openapi/anz-banking-products-api-openapi.yml
auth_types:
- apiKey
- mutualTLS
- none
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
mechanism_count: 6
method: searched
name: Anz Authentication
name_suffix: Authentication
oauth_flows: []
overview: Australia and New Zealand Banking Group (ANZ) secures its APIs with apiKey, mutualTLS, none, oauth2, and openIdConnect across 7 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Australia and New Zealand Banking Group (ANZ)
provider_slug: anz
scheme_count: 7
schemes:
- applies_to:
  - openapi/anz-cds-banking-products-openapi.yml#listBankingProducts
  - openapi/anz-cds-banking-products-openapi.yml#getBankingProductDetail
  name: PublicNoAuth
  note: Public Product Reference Data; version header x-v only.
  type: none
- applies_to:
  - non-PRD CDR banking operations (accounts, transactions, payees, payments, customer)
  flows:
  - flow: authorizationCode
    note: 'OIDC Hybrid/authorization-code flow with PAR (Pushed Authorization Requests), PKCE, and request objects per the CDR security profile. Authorization and token endpoints are published per data holder via the CDR Register / OIDC discovery, not in this product spec.

      '
  name: CDR-FAPI-OAuth2
  profile: FAPI 1.0 Advanced (Financial-grade API)
  scopes_ref: scopes/anz-scopes.yml
  type: oauth2
- name: CDR-OIDC
  note: OpenID Connect identity layer on top of the FAPI OAuth2 profile for the ADR consent flow.
  type: openIdConnect
- name: CDR-mTLS
  note: 'Holder-of-key mutual TLS (RFC 8705) binds access tokens to the ADR''s client certificate for all authenticated CDR resource calls; the CDS defines the MTLS server (mtls.dh.example.com placeholder in the shared spec).

    '
  type: mutualTLS
- docs:
  - https://developer.online.anz.com/How-it-works?path=FAQ
  - https://developer.online.anz.com/How-it-works?path=Sandbox
  flows:
  - client_authentication: private_key_jwt (client_assertion_type=urn:ietf:params:oauth:client-assertion-type:jwt-bearer, customer-signed JWT)
    flow: clientCredentials
    tokenUrl: https://api.fileactive.anz.com/auth/v2/oauth2/access_token
  name: Fileactive-OAuth2
  note: ANZ's OAuth 2.0 API is used for authentication and authorisation and is OpenID Connect compliant. The customers public key must be pre-exchanged for ANZ to verify the signed client credential grant.
  scopes_ref: scopes/anz-scopes.yml
  surface: 'ANZ Developer Portal (Fileactive) APIs: Payments, PayTo, Statements, FX, Confirmation of Payee, PayID Check'
  token:
    example_expires_in: 3600
    type: Bearer reference token
  type: oauth2
- header: apikey
  in: header
  name: Fileactive-apikey
  note: Sent on the token request and on every API call alongside the Bearer token; issued per App in the Sandbox.
  type: apiKey
- direction: inbound to the customer webhook
  header: apikey
  in: header
  name: Webhook-apikey
  note: ANZ authenticates webhook deliveries using an API key. The apikey header name and value are agreed with ANZ during onboarding.
  type: apiKey
slug: anz-authentication
source_filename: anz-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: searched\nsource: https://consumerdatastandardsaustralia.github.io/standards/#security-profile\ndocs: https://www.anz.com.au/support/legal/anz-apis/\nsummary:\n  types:\n  - apiKey\n  - mutualTLS\n  - none\n  - oauth2\n  - openIdConnect\n  tiers:\n  - name: Product Reference Data (public)\n    auth: none\n    note: 'The public PRD endpoints (GET /banking/products and /banking/products/{productId}) and the CDR discovery\n      endpoints (/discovery/status, /discovery/outages) require NO authentication. Only the mandatory x-v version\n      header is needed. Confirmed live returning HTTP 200 on both the ANZ (api.anz) and ANZ Plus (cdr.apix.anz)\n      brands.\n\n      '\n  - name: Consumer data sharing (CDR ADR model)\n    auth:\n    - oauth2\n    - openIdConnect\n    - mutualTLS\n    note: 'All non-PRD banking data (accounts, balances, transactions, direct debits, scheduled/regular payments,\n      payees, instalment plans, customer) is gated\
  \ behind the CDR security profile. Access is restricted to CDR-accredited\n      Data Recipients (ADRs) acting with explicit consumer consent obtained through the CDR consent/authorisation\n      flow.\n\n      '\nnotes: 'The harvested OpenAPI is the shared DSB Consumer Data Standards contract and expresses per-operation authorization\n  requirements via the x-scopes vendor extension rather than a components.securitySchemes block, so the mechanical\n  derive-authentication.py found no formal schemes. The auth model below is captured from the Consumer Data Standards\n  Security Profile (FAPI) and the ANZ Product APIs page.\n\n  '\nschemes:\n- name: PublicNoAuth\n  type: none\n  applies_to:\n  - openapi/anz-cds-banking-products-openapi.yml#listBankingProducts\n  - openapi/anz-cds-banking-products-openapi.yml#getBankingProductDetail\n  note: Public Product Reference Data; version header x-v only.\n- name: CDR-FAPI-OAuth2\n  type: oauth2\n  profile: FAPI 1.0 Advanced (Financial-grade API)\n\
  \  flows:\n  - flow: authorizationCode\n    note: 'OIDC Hybrid/authorization-code flow with PAR (Pushed Authorization Requests), PKCE, and request objects\n      per the CDR security profile. Authorization and token endpoints are published per data holder via the CDR\n      Register / OIDC discovery, not in this product spec.\n\n      '\n  scopes_ref: scopes/anz-scopes.yml\n  applies_to:\n  - non-PRD CDR banking operations (accounts, transactions, payees, payments, customer)\n- name: CDR-OIDC\n  type: openIdConnect\n  note: OpenID Connect identity layer on top of the FAPI OAuth2 profile for the ADR consent flow.\n- name: CDR-mTLS\n  type: mutualTLS\n  note: 'Holder-of-key mutual TLS (RFC 8705) binds access tokens to the ADR''s client certificate for all authenticated\n    CDR resource calls; the CDS defines the MTLS server (mtls.dh.example.com placeholder in the shared spec).\n\n    '\n- name: Fileactive-OAuth2\n  type: oauth2\n  surface: 'ANZ Developer Portal (Fileactive) APIs: Payments,\
  \ PayTo, Statements, FX, Confirmation of Payee, PayID\n    Check'\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.fileactive.anz.com/auth/v2/oauth2/access_token\n    client_authentication: private_key_jwt (client_assertion_type=urn:ietf:params:oauth:client-assertion-type:jwt-bearer,\n      customer-signed JWT)\n  token:\n    type: Bearer reference token\n    example_expires_in: 3600\n  note: ANZ's OAuth 2.0 API is used for authentication and authorisation and is OpenID Connect compliant. The customers\n    public key must be pre-exchanged for ANZ to verify the signed client credential grant.\n  scopes_ref: scopes/anz-scopes.yml\n  docs:\n  - https://developer.online.anz.com/How-it-works?path=FAQ\n  - https://developer.online.anz.com/How-it-works?path=Sandbox\n- name: Fileactive-apikey\n  type: apiKey\n  in: header\n  header: apikey\n  note: Sent on the token request and on every API call alongside the Bearer token; issued per App in the Sandbox.\n- name: Webhook-apikey\n\
  \  type: apiKey\n  in: header\n  header: apikey\n  direction: inbound to the customer webhook\n  note: ANZ authenticates webhook deliveries using an API key. The apikey header name and value are agreed with\n    ANZ during onboarding.\npayload_security:\n  jws: RS256 (FAQ) / PS512 (Sandbox page), 2048 or 4096\n  jwe: RSA-OAEP + A256GCM, 2048\n  object: secured_payload\n  source: https://developer.online.anz.com/How-it-works?path=FAQ\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anz/refs/heads/main/authentication/anz-authentication.yml
summary_line: apiKey/mutualTLS/none/oauth2/openIdConnect · 7 schemes
tags:
- Finance
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Product Reference Data
- ADI
---

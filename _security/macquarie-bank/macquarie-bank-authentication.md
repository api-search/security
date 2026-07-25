---
api_key_in: []
api_specs:
- filename: macquarie-bank-banking-account-balances-api-openapi.yml
  format: yaml
  label: Macquarie Bank Banking Account Balances API
  slug: macquarie-bank-banking-account-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macquarie-bank/refs/heads/main/openapi/macquarie-bank-banking-account-balances-api-openapi.yml
- filename: macquarie-bank-banking-account-direct-debits-api-openapi.yml
  format: yaml
  label: Macquarie Bank Banking Account Direct Debits API
  slug: macquarie-bank-banking-account-direct-debits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macquarie-bank/refs/heads/main/openapi/macquarie-bank-banking-account-direct-debits-api-openapi.yml
- filename: macquarie-bank-banking-account-scheduled-payments-api-openapi.yml
  format: yaml
  label: Macquarie Bank Banking Account Scheduled Payments API
  slug: macquarie-bank-banking-account-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macquarie-bank/refs/heads/main/openapi/macquarie-bank-banking-account-scheduled-payments-api-openapi.yml
- filename: macquarie-bank-banking-account-transactions-api-openapi.yml
  format: yaml
  label: Macquarie Bank Banking Account Transactions API
  slug: macquarie-bank-banking-account-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macquarie-bank/refs/heads/main/openapi/macquarie-bank-banking-account-transactions-api-openapi.yml
- filename: macquarie-bank-banking-accounts-api-openapi.yml
  format: yaml
  label: Macquarie Bank Banking Accounts API
  slug: macquarie-bank-banking-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macquarie-bank/refs/heads/main/openapi/macquarie-bank-banking-accounts-api-openapi.yml
- filename: macquarie-bank-banking-payees-api-openapi.yml
  format: yaml
  label: Macquarie Bank Banking Payees API
  slug: macquarie-bank-banking-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macquarie-bank/refs/heads/main/openapi/macquarie-bank-banking-payees-api-openapi.yml
- filename: macquarie-bank-banking-products-api-openapi.yml
  format: yaml
  label: Macquarie Bank Banking Products API
  slug: macquarie-bank-banking-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macquarie-bank/refs/heads/main/openapi/macquarie-bank-banking-products-api-openapi.yml
auth_types:
- none
- oauth2
- openIdConnect
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Macquarie Bank Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Macquarie Bank secures its APIs with none, oauth2, openIdConnect, and mutualTLS across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Macquarie Bank
provider_slug: macquarie-bank
scheme_count: 4
schemes:
- name: none
  sources:
  - public PRD + discovery endpoints
  type: none
- flows:
  - flow: authorizationCode
  name: oauth2
  sources:
  - CDR security profile
  type: oauth2
- name: openid-connect
  sources:
  - CDR security profile
  type: openIdConnect
- name: mutual-tls
  sources:
  - CDR security profile
  type: mutualTLS
slug: macquarie-bank-authentication
source_filename: macquarie-bank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: |\n  Australian Consumer Data Right (CDR) security profile / DSB Consumer Data\n  Standards (InfoSec) + Macquarie Open Banking page. The harvested CDS Banking\n  OpenAPI declares no inline components.securitySchemes (CDR security is defined\n  out-of-band by the standards), so this profile is authored from the published\n  CDR/CDS security model and Macquarie's data-holder implementation.\ndocs: https://www.macquarie.com.au/digital-banking/open-banking.html\nsummary:\n  types: [none, oauth2, openIdConnect, mutualTLS]\n  tiers:\n  - public-unauthenticated\n  - cdr-data-sharing\n  oauth2_flows: [authorizationCode]\ntiers:\n- name: public-unauthenticated\n  applies_to:\n  - Macquarie Bank CDR Product Reference Data API\n  - Macquarie Bank CDR Discovery Status API\n  auth: none\n  required_headers:\n  - name: x-v\n    description: Mandatory CDS API version header. Requests without it return HTTP 400\n      urn:au-cds:error:cds-all:Header/Missing.\n\
  \  note: Public PRD (Get Products / Get Product Detail) and CDS discovery status/outages\n    are openly callable over HTTPS with no credential, only the x-v version header.\n- name: cdr-data-sharing\n  applies_to:\n  - Macquarie Bank CDR Banking Data Sharing API\n  profile: FAPI 1.0 Advanced (CDR security profile)\n  schemes:\n  - name: openid-connect\n    type: openIdConnect\n    note: OIDC Hybrid flow; ID Token + authorization code.\n  - name: oauth2\n    type: oauth2\n    flows:\n    - flow: authorizationCode\n      note: Authorization Code with PKCE; Pushed Authorization Requests (PAR) required;\n        request objects signed (private_key_jwt client authentication).\n  - name: mutual-tls\n    type: mutualTLS\n    note: Access tokens are MTLS sender-constrained (RFC 8705). Client transport\n      certificates issued under the CDR PKI.\n  accreditation: Requires CDR Accredited Data Recipient (ADR) status registered on the\n    CDR Register plus explicit consumer consent. Not openly\
  \ callable.\nschemes:\n- name: none\n  type: none\n  sources: [public PRD + discovery endpoints]\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n  sources: [CDR security profile]\n- name: openid-connect\n  type: openIdConnect\n  sources: [CDR security profile]\n- name: mutual-tls\n  type: mutualTLS\n  sources: [CDR security profile]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/macquarie-bank/refs/heads/main/authentication/macquarie-bank-authentication.yml
summary_line: none/oauth2/openIdConnect/mutualTLS · 4 schemes
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Data Right
- Consumer Banking
- Australia
- Product Reference Data
- Payments
---

---
api_key_in: []
auth_types:
- oauth2
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Navy Federal Credit Union Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Navy Federal Credit Union secures its APIs with oauth2 and mutualTLS across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Navy Federal Credit Union
provider_slug: navy-federal-credit-union
scheme_count: 2
schemes:
- description: 'Member-consented OAuth authorization: the member authenticates and grants a third party consent, producing an access token scoped to the consented accounts/data products in the Open Banking API Catalog. Client registration and token management are handled through the API Management API.'
  documented_flow: authorizationCode
  name: OAuthMemberConsent
  sources:
  - developer portal documentation
  type: oauth2
- description: Gateway connectivity requires mutual TLS with client-certificate whitelisting; the Gateway Connectivity API is provided to prove out a working mTLS request before consuming data-access products.
  name: MutualTLS
  sources:
  - developer portal documentation
  type: mutualTLS
slug: navy-federal-credit-union-authentication
source_filename: navy-federal-credit-union-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: https://developer.navyfederal.org/open-banking-api-catalog.html\ndocs: https://developer.navyfederal.org/document-library.html\nnote: >-\n  Navy Federal's Open Banking API Catalog is partner-gated and publishes no\n  downloadable OpenAPI/Swagger pre-login, so this profile is derived from the\n  documented access model on the developer portal rather than machine-read from\n  a securitySchemes block. Access requires third-party registration plus a\n  signed Data Access Agreement before credentials are issued.\nsummary:\n  types: [oauth2, mutualTLS]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  consumer_permissioned: true\nschemes:\n- name: OAuthMemberConsent\n  type: oauth2\n  documented_flow: authorizationCode\n  description: >-\n    Member-consented OAuth authorization: the member authenticates and grants a\n    third party consent, producing an access token scoped to the consented\n    accounts/data products in\
  \ the Open Banking API Catalog. Client registration\n    and token management are handled through the API Management API.\n  sources: [developer portal documentation]\n- name: MutualTLS\n  type: mutualTLS\n  description: >-\n    Gateway connectivity requires mutual TLS with client-certificate\n    whitelisting; the Gateway Connectivity API is provided to prove out a\n    working mTLS request before consuming data-access products.\n  sources: [developer portal documentation]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/navy-federal-credit-union/refs/heads/main/authentication/navy-federal-credit-union-authentication.yml
summary_line: oauth2/mutualTLS · 2 schemes
tags:
- Financial-Services
- Banking
- United States
- Credit Union
- Open Finance
- Open Banking
- Data Aggregation
- Payments
---
